# Android WebView App Setup Guide

Follow these steps to set up and customize the WebView Android application in Android Studio.

## 1. Import the Source Code
- Open **Android Studio**.
- Click on **File > Open**.
- Select the project folder and click **OK**.

## 2. Change the Package Name
- In **Android Studio**, go to `AndroidManifest.xml`.
- Find the **package name** at the top and update it.
- Refactor the package name in the Java/Kotlin files:
  - Right-click on the old package name in **Java** directory.
  - Click **Refactor > Rename**.
  - Enter the new package name and apply the changes.

## 3. Change Your Web URL in `MainActivity.java`
- Open `MainActivity.java`.
- Locate the following line:
  ```java
  String websiteURL = "https://yourwebsite.com";
  ```
- Replace `https://yourwebsite.com` with your desired web URL.

## 4. Update `google-services.json`
- Replace the existing `google-services.json` file (located in `app/` directory) with your own Firebase **google-services.json**.

## 5. Change Your OneSignal App ID
- Open `ApplicationClass.java`.
- Find the line where **OneSignal App ID** is defined:
  ```java
  OneSignal.initWithContext(this);
  OneSignal.setAppId("YOUR_ONESIGNAL_APP_ID");
  ```
- Replace `YOUR_ONESIGNAL_APP_ID` with your actual OneSignal App ID.

## 6. Update the App Name in `strings.xml`
- Open `res/values/strings.xml`.
- Find the line:
  ```xml
  <string name="app_name">YourAppName</string>
  ```
- Replace `YourAppName` with your desired app name.

## 7. Build and Run the Application
- Click **Build > Make Project**.
- Connect a real device or use an emulator.
- Click **Run** to launch the app.

🎉 **Happy Coding!** 🚀

