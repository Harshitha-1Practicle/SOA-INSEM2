# MockMvc MSL Controller Testing

A small Spring Boot project for the controller-testing experiment.

## Requirements
- JDK 17 or later
- Maven 3.6+ (or import the project into an IDE with Maven support)
- Internet access the first time Maven downloads dependencies

## Run the test

From this project folder, run:

```bash
mvn test
```

In Eclipse:
1. Import the extracted folder using **File > Import > Existing Maven Projects**.
2. Select the project folder and click **Finish**.
3. Open `MSLControllerTest.java`.
4. Right-click the file and choose **Run As > JUnit Test**.

In IntelliJ IDEA:
1. Open the extracted project folder.
2. Allow Maven to load dependencies.
3. Open `MSLControllerTest.java` and click the green run icon beside the test.

## What the test checks
It sends a simulated GET request to `/msl/add` with `a=5` and `b=10`, then checks:
- HTTP status is `200 OK`
- Response body is `15`

The test uses `@WebMvcTest` and `MockMvc`, so it tests the web layer without starting a real HTTP server.
"# SOA-INSEM2" 
