FROM openjdk:17
WORKDIR /app

# JAR 파일명을 변수로 받아서 복사
ARG JAR_FILE
COPY ${JAR_FILE} app.jar

ENTRYPOINT ["java", "-jar", "app.jar"]
