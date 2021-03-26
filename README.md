

Note: These instructions were made for Windows 10. Exact steps may vary by platform.


## Installing Flutter & Android Studio
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

   - **Mac**:
      - a

   - To confirm the path was added correctly, open up a terminal and type in the followng commands:
       - `flutter --version`
       - `dart --version`
   - These should show the SDK versions for both flutter and dart. Ask for help if you did not get this result.

## Creating a new project
- launch Android Stuido
- select "Create New Flutter project"
- select "Flutter application"
- Choose an empty folder to use for your project (just like for IntelliJ)
- Name it whatever you want, but make sure the package name is `com.example.yourprojectname`
  - This is typically related to the project's website, but since we don't have one, we can leave it as example.
- You should now have a new Flutter project!

### Running our project
- Open the project folder in your terminal of choice (Android Studio has one built in)
- run `flutter doctor`. This will reveal steps we need to follow before we can run the project.
  - sign the Android Studio licenses
  - Potential issues:
    - `Android Studio [not installed]`
      - Flutter does now know the correct path to your Android Stuido install.
      - This may be set manually with `flutter 
