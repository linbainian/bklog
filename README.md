### 技术选型：
* JDK8
* 数据库MySQL
* 主框架 (Spring-boot、Spring-data-jpa）
* 安全权限 Shiro
* 搜索工具 Lucene
* 缓存 Ehcache
* 视图模板 Freemarker
* Bootstrap 前端框架

### 启动：
 - 项目默认配置是在容器中启动(个人习惯), 如果想要main方法运行, 请自行修改
 ```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
    <exclusions>
        <!-- 容器启动,启用下面代码. main 方法运行注释此处
        <exclusion>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-tomcat</artifactId>
        </exclusion>
        -->
    </exclusions>
</dependency>
```
- 启动成功后访问： http://localhost:8080/

![image](https://github.com/linbainian/bklog/blob/master/mblog/1.jpeg)
