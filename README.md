📱 Facebook Testing With Appium

Automated UI Testing for the Facebook Android Application using Appium and Java.

🚀 Overview

This project focuses on automating the Facebook Android App using Appium.
It demonstrates how to launch the app, interact with UI elements, inspect components, and run automated Android test flows.

This repository is ideal for:

QA Engineers

Automation Testers

Students learning Mobile Automation

🧩 Features

✔ Automates Facebook Android App

✔ Works on real devices & emulators

✔ Uses Appium + Java

✔ Clean project structure

✔ Extendable for more scenarios

✔ Uses Desired Capabilities for configuration

🛠 Tech Stack
Component	Purpose
Appium	Mobile UI Automation
Java	Test scripting
Android Studio	SDK, Device Manager
TestNG / JUnit	Test execution
Maven	Dependency management
ADB	Device communication
Appium Inspector	Inspecting UI elements
📦 Project Structure
FacebookTestingWithAppium/
│
├── src/
│   ├── test/java/
│   │   ├── base/
│   │   ├── pages/
│   │   └── tests/
│   │
│   └── main/resources/
│
├── pom.xml
└── README.md

📱 Prerequisites

Make sure you have:

Java JDK 8 or above

Android Studio

Node.js

Appium Server (GUI or CLI)

Appium Inspector

USB Debugging enabled

Real device or emulator

🔧 Installation
1️⃣ Clone the repository
git clone https://github.com/your-username/FacebookTestingWithAppium.git

2️⃣ Install dependencies (Maven)

Add inside pom.xml:

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

⚙ Appium Desired Capabilities
caps.setCapability("platformName", "Android");
caps.setCapability("deviceName", "Android Device");
caps.setCapability("automationName", "UiAutomator2");
caps.setCapability("appPackage", "com.facebook.katana");
caps.setCapability("appActivity", "com.facebook.katana.LoginActivity");
caps.setCapability("noReset", true);

▶️ How to Run the Tests
1️⃣ Start Appium Server
appium

2️⃣ Connect the device
adb devices


You should see your device listed.

3️⃣ Run the tests
mvn clean test

🎯 What This Project Demonstrates

Launching the Facebook app using Appium

Interacting with Android UI elements

Inspecting elements with Appium Inspector

Using waits (implicit & explicit)

Setting Desired Capabilities

Automating basic flows

Understanding Facebook app UI structure

📚 Facebook App Components Covered

Opening the app

Locating elements

Clicking buttons

Typing inside input fields

Navigation within screens

Handling dynamic UI elements

🧱 Future Enhancements

Add video recording

Add Allure / Extent reporting

Add CI/CD (GitHub Actions)

Add parallel execution

Add cross-device support

Add cloud device execution (BrowserStack, LambdaTest)

🧑‍💻 Author

Mohit Dayma
Mobile Automation Enthusiast
📍 India
