### Sample Spring Boot app to connect to SQL Database 

## Steps:
- Update HelloController.java with the database credentials

```java
		String connectionUrl =
                "jdbc:sqlserver://yourserver.database.windows.net:1433;"
                        + "database=AdventureWorks;"
                        + "user=yourusername@yourserver;;"
                        + "password=***;"
                        + "encrypt=true;"
                        + "trustServerCertificate=false;"
                        + "loginTimeout=30;";
```                        
- mvn clean package
- cd target
- java -jar JARFILENAME

- Access localhost:8080/test, to check if the connection is working.