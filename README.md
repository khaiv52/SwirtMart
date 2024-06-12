# SwirtMart
SwirtMart is a Flutter shopping app project focused on the e-commerce topic, implemented by a team of three members: Khải, Thanh Hiền, and Ngọc Hiền.

# Steps to Set Up and Run the Project
### Step 1: Update Firebase Configuration
#### 1.1. Create a New Firebase Project
+ Create a Firebase Project: Go to the Firebase Console and create a new project or use an existing one.
+ Add Apps to Your Project: Add your Android and iOS apps to your Firebase project. This will generate the necessary configuration files (google-services.json for Android and GoogleService-Info.plist for iOS).
#### 1.2. Download Configuration Files
+ Android: Download the google-services.json file.
+ iOS: Download the GoogleService-Info.plist file.
#### 1.3. Update Your Flutter Project with the New Configuration Files
- Android:
  - Remove the Old google-services.json File: Delete the old google-services.json file from the android/app directory.
  - Add the New google-services.json File: Place the new google-services.json file into the android/app directory.
- iOS:
  - Remove the Old GoogleService-Info.plist File: Delete the old GoogleService-Info.plist file from the ios/Runner directory.
  - Add the New GoogleService-Info.plist File: Place the new GoogleService-Info.plist file into the ios/Runner directory.
### Step 2: Import backup.json Using AppConfig.json: This file contains the API key to enable access to the Firestore service.
- Open Command Line: Navigate to the directory containing backup.json and AppConfig.json.
- Run command: 
```
npx -p node-firestore-import-export firestore-import -a appConfig.json -b backup.json
```
### Step 3: Add Dependencies in Flutter
- Open pubspec.yaml: In your project directory, find and open the pubspec.yaml file.
- Fetch Dependencies: Click "Pub get" to install necessary dependencies.
### Step 4: Configure Project SDK
- Open Project Structure:
  - Press Ctrl + Alt + Shift + S or navigate to File -> Project Structure.
- Select SDK Version:
  - Go to the Project section, and select the appropriate SDK version.
- Enable Dart and Flutter Plugins:
  - In the Modules section, ensure that Dart SDK, Dart Packages, and Flutter Plugins are selected.
 ### Step 5: Run application
- Run the application using the command:
```
Flutter run
```
- Alternatively, click the start icon to run the application.

### Additional Notes
- Android SDK: Ensure the Android SDK is installed.
- Environment PATH: Add Flutter to the Environment PATH for proper functioning.
