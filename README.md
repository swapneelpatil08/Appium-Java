# Appium-Java Project

This automation project uses Appium and Java, to automate given Monefy application. <br />

# Pre-requisites
- Java _v8_
- [Appium Server UI](https://github.com/appium/appium-desktop/releases "Releases · appium/appium-desktop") _v1.22.0_
- [Appium Inspector](https://github.com/appium/appium-inspector/releases "Releases · appium/appium-inspector") _v2021.9.2_
- [Android Studio](https://developer.android.com/studio "Download Android Studio and SDK tools  |  Android Developers") _v2020.3.1_
- IntelliJ IDEA

# Setup
- Create Android virtual device from Android Studio: _Pixel XL API 30_
    - Device name: _Pixel XL_
    - Android version: _"R" API 30_
    - AVD Name: _Pixel XL API 30_
- Configure Java path in Appium server.
  ![Appium Server UI Config Screenshot](https://i.imgur.com/UUFC6QC_d.webp?maxwidth=760)
  
# Installation
1. Clone repository by executing below command <br /> `git clone https://github.com/swapneelpatil08/swapneel-patil.git`
2. Open `monefyAppiumTest` from cloned repository in IntelliJ IDEA.
3. Download dependencies by running below command <br /> `./gradlew build`

# Project Structure

## Tests
Spec files are placed in directory `src/test/java/`. Currently, this project has 2 spec files and total of 3 tests.

## Page Objects
This framework use Page Object Model _(aka POM)_, design pattern that creates object repository for storing web elements. Page Objects are located at `src/main/java/PageObjects/`.

## Resources
Apk required for testing is kept under the `src/main/resources/`

## Locators 
In this project below locator strategies are used:
1. _id_
2. _xPath_
3. _accessibility_

## Run tests
1. Open and start Appium Server UI.
   ![Appium Server UI Screenshot](https://i.imgur.com/ta05RAb_d.webp?maxwidth=1520)
2. Now you are all set to run the tests, execute below command to run tests <br /> `./gradlew test`

# Reporting
This framework uses in-build jUnit reporter. <br />
![JUnit Report](https://i.imgur.com/IqNfF9k_d.webp?maxwidth=1520)