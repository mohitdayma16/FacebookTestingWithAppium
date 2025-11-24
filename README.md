#📱 Facebook Testing With Appium

Automated UI Testing for the Facebook Android Application using Appium & Java

🚀 Overview

This project is focused on automating the Facebook Android mobile application using Appium and Java.
It demonstrates how to:

Launch the Facebook app

Interact with mobile UI elements

Use Appium Inspector to locate elements

Execute automated test flows

Validate Facebook app behavior on Android devices

This repository is ideal for QA engineers, automation testers, and students learning mobile automation.

🧩 Features

✔ Automates Facebook Android application
✔ Works on real devices and emulators
✔ Uses Appium + Java
✔ Supports Android 8+
✔ Uses Desired Capabilities for easy configuration
✔ Follows a clean project structure
✔ Highly extendable

🛠 Tech Stack
Component	Purpose
Appium	Mobile UI Automation
Java	Automation scripting
TestNG / JUnit	Test execution
Maven/Gradle	Dependency management
ADB (Android Debug Bridge)	Device communication
Appium Inspector / UIAutomator Viewer	Element inspection
Android Studio	SDK, Tools, Emulator
📦 Project Structure
FacebookTestingWithAppium/
│
├── src/
│   ├── test/java/
│   │   ├── base/
│   │   │   └── BaseTest.java
│   │   ├── pages/
│   │   └── tests/
│   │
│   └── main/resources/
│
├── pom.xml
└── README.md

📱 Prerequisites

Make sure the following tools are installed:

🔧 Required Tools

Java JDK 8 or above

Android Studio

Appium Server (Desktop or CLI)

Appium Inspector

Node.js & NPM

USB Debugging enabled on device

A real Android device or emulator

📦 Installation
1. Clone the repository
git clone https://github.com/your-username/FacebookTestingWithAppium.git

2. Install dependencies (Maven)

Add this to pom.xml:

<dependencies>
    <dependency>
        <groupId>io.appium</groupId>
        <artifactId>java-client</artifactId>
        <version>8.5.1</version>
    </dependency>
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version>7.9.0</version>
    </dependency>
</dependencies>

⚙ Appium Configuration (Desired Capabilities)

These are the capabilities required to launch the Facebook app:

caps.setCapability("platformName", "Android");
caps.setCapability("deviceName", "Android Device");
caps.setCapability("automationName", "UiAutomator2");
caps.setCapability("appPackage", "com.facebook.katana");
caps.setCapability("appActivity", "com.facebook.katana.LoginActivity");
caps.setCapability("noReset", true);

▶️ How to Run
Step 1: Start Appium Server
appium

Step 2: Connect Android Device
adb devices


Ensure your device appears in the list.

Step 3: Run Tests
mvn clean test

🎯 What This Project Demonstrates

This project covers:

Launching Facebook app using Appium

Interacting with UI elements

Locating elements using Inspector

Handling waits & timeouts

Basic flow automation

Understanding the Facebook app structure

Best practices for Android automation

📚 Facebook App Components Covered

App launch and verification

Finding elements using IDs, XPaths

Entering text in input fields

Clicking buttons

Navigating screens

Understanding Facebook’s UI hierarchy

🧱 Future Enhancements

🔹 Add Allure or Extent Reports
🔹 Add parallel execution
🔹 Add CI/CD integration (GitHub Actions)
🔹 Add support for iOS
🔹 Add screen recording during tests
🔹 Add cloud device execution (BrowserStack, LambdaTest)

🧑‍💻 Author

Mohit Dayma
Automation & Android Enthusiast
📍 India
