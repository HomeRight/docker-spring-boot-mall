FROM maven:3-jdk-11
ENV DB_HOST_IP="107.167.179.137"
WORKDIR /usr/src/app
COPY . ./
COPY wait-for-it.sh ./wait-for-it.sh
RUN chmod +x wait-for-it.sh
RUN mvn clean package
CMD java -jar target/springboot-mall-0.0.1-SNAPSHOT.jar

