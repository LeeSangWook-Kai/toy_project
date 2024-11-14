# toy_project
토이 프로젝트를 하기 위한 Repository 2024

## 환경설정
### SpringBoot3 - Spring Security 6, Mybatis, Mysql, Thymeleaf, JDBC API, Spring Web, Spring Batch, devtool
### Javascript, Jquery, Bootstrap 5, Font Awesome(https://fontawesome.com/icons), Matrial UI(https://m2.material.io/design/color/the-color-system.html#tools-for-picking-colors), Jquery UI, Masonry (https://getbootstrap.com/docs/5.0/examples/masonry/)
### ER-D : draw.io
### Wireframe : Figma
### IDE : Intellij Ultimate
### Source Repository : Github

## Application.yml
spring:
  application:
    name: TtoT
  devtools:
    restart:
      enabled: true
  datasource:
    url: jdbc:mysql://localhost:3306/project?useSSL=false&serverTimezone=UTC&characterEncoding=UTF-8
    driver-class-name: com.mysql.cj.jdbc.Driver
    username: XXXX
    password: XXXX
  
  servlet:
    multipart:
      enabled: true
      #      location: D:\\springbootWithAws\\myProfile\\src\\main\\resources\\static\\upload\\
      max-file-size: 10MB
      max-request-size: 30MB

uploadfile.dir: D:\\springbootWithAws\\myProfile\\src\\main\\resources\\static\\upload\\
movingfile.from: profile\\temp\\
movedfile.to: profile\\

mybatis:
  mapper-locations: classpath:mapper/*.xml

logging:
  level:
    org.springframework.jdbc: debug
    org.apache.coyote.http11: trace
    org.k8go4go.miniboard.mapper: trace


server:
  servlet:
    context-path: /
