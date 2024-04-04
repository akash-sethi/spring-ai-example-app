```bash
git clone https://github.com/akash-sethi/spring-ai-example-app.git
```

# Build

Install [Maven](https://www.maven.org) and JDK 21. If you use SDKMan you can run the command below:

```bash
sdk install java 21.0.2-tem
```

```bash
./mvnw spring-boot:run
```

Check Health
```bash
curl http://localhost:8080/actuator/health
```

API
```bash
curl -X GET "http://localhost:8080/chatbot/story?subject=Frankenstein"
```

```bash
curl --header "Content-Type: application/json" \
--request POST \
--data '{"question":"what is pdf"}' \
http://localhost:8080/chatbot/ask
```

