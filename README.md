

Note: These instructions were made for Windows 10. Exact steps may vary by platform.


## Installing Flutter
1. visit https://flutter.dev/docs/get-started/install/
   - Choose the correct instructions for your device
   - *This guide echoes most of the instructions here, so feel free to follow either one!*
2. Follow the instructions to install the flutter SDK
   - **IMPORTANT**: Take note of the exact install path, because we need to reference it!
3. Add the flutter SDK to your environment variables path
   - **Windows**:
     - search "environment variables" in the Start search bar and click the first option
     - on the following screen, click "Environment Variables..."
     - under "User variables for [your username]", scroll down to and highlight "Path", then click "Edit..."
     - clich "New" on the right and paste in the path to the Flutter SDK  
       e.g. `C:\path\to\flutter\bin`

   - *Mac and Linux instructions can be found in the official Flutter guide*

   - To confirm the path was added correctly, open up a terminal and type in the followng commands:
       - `flutter --version`
       - `dart --version`
   - These should show the SDK versions for both flutter and dart. Ask for help if you did not get this result.

## Installing Android Studio
- Go to https://developer.android.com/studio and follow the install instructions.


## Creating a new project
1. launch Android Stuido
2. select "Create New Flutter project"
3. select "Flutter application"
4. Choose an empty folder to use for your project (just like for IntelliJ)
5. Name it whatever you want, but make sure the package name follows the `com.example.yourprojectname` format.
   - This is typically related to the project's website. Since we don't have one, we can leave it as example.
6. You should now have a new Flutter project!

## Adding Flutter & Dart Plugins
- IMPORTANT: Flutter will not be able to build without adding these plugins to Android Stuido
1. In Android Studio, navigate to File -> Settings -> Plugins
2. Look up and install the official plugins for Flutter and Dart, respectively (should be the only ones that appear)

## Running our project
1. Open the project folder in your terminal of choice (Android Studio has one built in)
2. run `flutter doctor`. This will reveal steps we need to follow before we can run the project.
3. Android licenses must be signed before you can run your Android app. To sign them run: `flutter doctor --android-licenses`, then enter `y` for each license.
4. Other potential issues:
   - `Android Studio [not installed]`
     - Flutter does now know the correct path to your Android Stuido install.
     - This may be set manually with `flutter config --android-studio-dir="C:\Program Files\Android\Android Studio"`
   - `No connected devices`/`No devices available`
     - In Android Studio, navigate to File -> Project Structure -> Project -> Project SDK
     - If already have an Android SDK, choose that. (I have Android API 30, for example)
     - If none are listed, follow these steps:
       - In Android Studio, navigate to Tools -> SDK manager, and select one of the available platforms.
       - Note: Higher API levels mean more features, but less compatibility with Android devices.
5. Select an Android device from the dropdown in the top right
   - If you have an Android phone, you may simply connect it to your computer. Android Studio will automatically detect it.
   - Otherwise, you may download an Android emulator
     - In Android Studio, navigate to Tools -> AVD Manager -> Create Virtual Device...
     - Select an Android phone from the list (i.e. Pixel 3).
     - Download the most recent image and select Next
     - Click finish.
     - **Note that Android emulators are resourse expensive, and may be slow on some computers.**
6. Click run!

## Flutter Lab
- When you created your Flutter project, a README.md was generated. Open it up and follow the instructions for "Lab: Write your first Flutter app".
- Alternatively, go to: https://flutter.dev/docs/get-started/codelab

