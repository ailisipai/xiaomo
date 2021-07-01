# Getting Started

### Reference Documentation

For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.5.2/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.5.2/maven-plugin/reference/html/#build-image)
* [Eureka Server](https://docs.spring.io/spring-cloud-netflix/docs/current/reference/html/#spring-cloud-eureka-server)
* [Java Mail Sender](https://docs.spring.io/spring-boot/docs/2.5.2/reference/htmlsingle/#boot-features-email)
* [MyBatis Framework](https://mybatis.org/spring-boot-starter/mybatis-spring-boot-autoconfigure/)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/2.5.2/reference/htmlsingle/#using-boot-devtools)

### Guides

The following guides illustrate how to use some features concretely:

* [Service Registration and Discovery with Eureka and Spring Cloud](https://spring.io/guides/gs/service-registration-and-discovery/)
* [MyBatis Quick Start](https://github.com/mybatis/spring-boot-starter/wiki/Quick-Start)

### 配置mybatis的逆向工程
* 配置数据库链接信息
    > 数据库驱动 
    > 
    > 数据库地址：注意逆向工程可能需要配置时区
    > 
    > 数据库链接用户名和密码
    > 
    > 数据库驱动本地配置：mysql-connector-java-8.0.22.jar\
* 配置逆向工程配置文件
  * 引入链接属性文件
    ```
    <properties resource=xxxx.properties></properties>
    ```
  * 指定数据库链接的驱动
    ```
    <classPathEntry location="${jdbc.driverLocation}"/>
    ```