API Testing Project with TestNG and RestAssured**  

This project demonstrates API testing using TestNG and RestAssured. It focuses on implementing temporary solutions, addressing technical debt, and following best practices for isolating and documenting problematic code.  
1. Project Setup
1.1 Prerequisites 
Before running this project, ensure the following tools are installed:  
Java JDK 8 or higher
Apache Maven
An IDE (e.g., IntelliJ IDEA or Eclipse)  

1.2 Clone or Download the Project
1. Clone the repository or download it as a ZIP file:  
   bash
   git clone (https://github.com/Rapatel0936/RutulKumar_Patel_8990936_A4.git)
   
2. If downloaded as a ZIP file, extract it to a folder of your choice.  

1.3 Import the Project into an IDE
1. Open your IDE.  
2. Select **Import Project** or **Open Project**.  
3. Choose the folder containing the project files.  
4. Wait for Maven to resolve all dependencies.  

**2. Running the Tests**  

**2.1 Test Suite Configuration**  
The tests are managed using a TestNG suite. The configuration file is named testng.xml.  

**2.2 Running the Tests via IDE**  
1. Locate the `testng.xml` file in your project.  
2. Right-click on the file and select **Run testng.xml**.  

**2.3 Running the Tests via Maven**  
1. Open a terminal and navigate to the project directory.  
2. Run the following command:  
   mvn test

**3.1 Key Files and Folders**  
- src/test/java/com.example.api/ApiTest.java: Contains the test cases for the API.  
- testng.xml: TestNG configuration file that defines the test suite and test classes.  
- pom.xml: Maven configuration file with the dependencies for TestNG and RestAssured.  
- README.md: This documentation file.  

## **4. Test Cases**  

### **4.1 Current Test Cases**  
1. **GET Request Test**:  
   Verifies the status code and basic content of a response from a public API.
   
3. **GET All Posts Test**:  
   Validates the response of fetching multiple posts.

4. **POST Request Test**:  
   Verifies the creation of a new resource using a POST request.

**4.2 Planned Improvements**  
- Validate the response structure more thoroughly.  
- Add tests for handling errors and edge cases.  
- Implement data-driven tests for dynamic input.
  
**5. Dependencies**  

**Maven Dependencies**  
The project uses the following libraries:  
1. **TestNG**: For writing and running tests.  
2. **RestAssured**: For making API requests and validating responses.  

The dependencies are defined in pom.xml:  
**pom.xml**
<dependencies>
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version>7.4.0</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>io.rest-assured</groupId>
        <artifactId>rest-assured</artifactId>
        <version>4.4.0</version>
    </dependency>
</dependencies>

**6. Known Issues and Technical Debt**  

**6.1 Temporary Solutions**  
**GET Request Test**: Currently, only the status code is validated. Improvements planned:  
Validate the response body structure.  
Add checks for specific fields and values.  

**6.2 Technical Debt**  
**POST Request Test**: The test lacks detailed error handling and response validation.
