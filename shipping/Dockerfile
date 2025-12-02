FROM maven:3.9.11 AS builder
EXPOSE 8080
WORKDIR /opt/server
COPY pom.xml .
COPY src ./src
RUN mvn clean package
RUN mv target/shipping-0.0.1-SNAPSHOT.jar shipping.jar
ENV CART_ENDPOINT="cart:8080" \
    DB_HOST="mysql"
CMD ["java", "-jar","shipping.jar"] 
CMD ["sleep", "10000"]  

