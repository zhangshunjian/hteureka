FROM java:8
MAINTAINER "yinhaijing"<304814585@qq.com>
#定义时区参数
ENV TZ=Asia/Shanghai
ADD ht-eureka-0.0.1-SNAPSHOT.jar app.jar
RUN bash -c 'touch /app.jar'
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom", "-Dspring.profiles.active=dev",  "-jar","/app.jar"]

