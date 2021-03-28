[![N|Solid](https://www.bobit.us/images/bobit-logo.png)](https://bobit37.github.io/Resume/)

# WebdriverTestCases

## Prerequisites

- Docker
- Git
- Java
- Selenium WebDriver
- Chrome Driver
- IDE

## Steps

- Pull Docker image for the-internet app:
```
docker pull gprestes/the-internet
```

# WebdriverTestCases

- This project has been created Page Object Model (POM) approach using Maven and TestNG.
- Allure report, extent report can be generated.
- Screenshot listener is cretaed to take screentshot if test case is failed. In framework target > surefire-reports > failure_screenshots
- Another taking screenshot is put in Allure listener. Project > screenthots
- All log files are stored in logs folder > application.properties.
- This framework is compatible with parallel execution and just configure in testng_runner.xml
- Apache POI jar is added for parameterized testing and excelutil is created to read data from excel sheet. In LoginPageTest class, invalid credentials test case is created using parameterized approach and all data is got from excel data file.

## Local usage: Clone framework 

- To use framework, copy https://github.com/BobIT37/WebdriverTestCases.git and clone in Eclipse or INtellij IDEA

## Using command line
## Specify project path on the terminal
- cd project path

## to execute all test cases in a class
- mvn -Dtest=LoginPageTest test

## to execute specific test method in a class
- mvn -Dtest=LoginPageTest#testPageTitleTest test
- mvn -Dtest=LoginPageTest#testLoginValidCreds test
- mvn -Dtest=LoginPageTest#testLoginInvalidCreds test

## without command line
- go to test resources and find runner package, then execute testngrunner.xml file

# Reports

## Extent Report
https://bobit37.github.io/extentreport/

## Emailable HTML Report
https://bobit37.github.io/htmlreport/

## Allure Report
- cd project path
- run command: allure serve allure-results
