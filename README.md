# Coding Assessment POC

Functional tests for the Selendroid App

## Test Cases

- Create a new user
- Assert the values on Verfiy screen

## Installation

The following tools must be installed to run the test cases:

```
Install JDK
Install IntelliJ IDEA / Eclipse
Install Cucumber Feature Plugin
Install Android SDK
Install Android API version 4.4.2
Install Appium for Windows / Mac
Install Android Studio
Install Node JS
```

## Setup

- Open the project in the IDE of your choice.
- Launch `Appium` server.
- Create a new android emulator with at least API 26

## Running the tests

- You need to modify `src/main/java/com/apium/poc/config/config.properties` and replace `DEVICE_NAME`, `EMU_NAME` with your corresponding running device name.
- For Mac users, in `POC/src/main/java/com/apium/poc/utilities/XlsReader.java` modify the `new XlsReader` object path at the bottom of the file to meet the directory of your porject.
- You can either execute `mvn test` or open `POC/src/test/java/com/apium/poc/Runner/TestRunner.java`, right click and then `Run 'TestRunner'`

_Note:_ The tests will execute once their is a single test data record in the data file placed at `POC/src/main/java/com/apium/poc/utilities/testdata/Test_Data_new.xlsx`

## Reporting

Report will be generated in `/POC/target/cucumber-html-report`
