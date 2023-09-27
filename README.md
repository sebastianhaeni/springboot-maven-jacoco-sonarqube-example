# Example Springboot Project + Jacoco Coverage + SonarQube

Follow these steps to generate the coverage report and send it to SonarQube:

First, start SonarQube:

```bash
docker compose up -d
```

Then, login to http://localhost:9000 with admin/admin credentials.
Change the password to `sonar`.

Lastly, run the following command to generate the coverage report and send it to SonarQube:

```bash
mvn test jacoco:report sonar:sonar
```
