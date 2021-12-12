# Config Service

## REST API

* Monitoring        

| Endpoint	                  | Method   | Status | Description    		   	                        |
|:---------------------------:|:--------:|:------:|:-----------------------------------------------:|
| `/actuator/info`            | `GET`    | 200    | Get info of service.                            |
| `/actuator/health`          | `GET`    | 200    | Get health of service.                          |
| `/actuator/health/readiness`| `GET`    | 200    | Get readiness state of service.                 |
| `/actuator/health/liveness` | `GET`    | 200    | Get liveness state of service.                  |
| `/actuator/flyway`          | `GET`    | 200    | Get config of flyway.                           |
| `/actuator/prometheus`      | `GET`    | 200    | Get Prometheus metrics of service.              |
| `/actuator/metrics`         | `GET`    | 200    | Get all metrics of service.                     |


## Useful Commands

| Gradle Command	                 | Description                                                  |
|:-----------------------------------|:-------------------------------------------------------------|
| `./gradlew bootRun`                | Run the application.                                         |
| `./gradlew build`                  | Build the application.                                       |
| `./gradlew build -x test`          | Build the application and omit test.                         |
| `./gradlew test`                   | Run tests.                                                   |
| `./gradlew bootJar`                | Package the application as a JAR.                            |
| `./gradlew bootBuildImage`         | Package the application as a container image.                |
| `./gradlew bootBuildImage -x test` | Package the application as a container image and omit test.  |

After building the application, you can also run it from the Java CLI:

```bash
java -jar build/libs/config-service-0.0.1-SNAPSHOT.jar
```
