# OpenJDK 17 이미지 사용
FROM openjdk:17
WORKDIR /app

# JAR 파일 복사 (빌드 후 target 폴더에 생성됨)
COPY target/*.jar app.jar

# Cloud Run은 $PORT에서 실행해야 하므로 환경 변수 설정
ENV PORT=8080
EXPOSE 8080

# JAR 실행
CMD ["java", "-jar", "app.jar"]