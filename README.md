# Expo Android Build Failure: ':app:processDebugGoogleServices' Error

This repository demonstrates a common error encountered when building Android APKs with Expo CLI.  The error, `Execution failed for task ':app:processDebugGoogleServices'`, typically stems from issues with the Firebase configuration file (`google-services.json`).  This can happen if the file is missing, outdated, or contains mismatched configurations.

The `bug.js` file contains an example of an app setup that might trigger this issue (it simulates missing Firebase configuration). The `bugSolution.js` provides a fix by ensuring the correct `google-services.json` file is in place and the configuration matches the app's Firebase setup.

**To reproduce the bug:**
1. Clone this repository.
2. Follow the instructions to install dependencies.
3. Try to build an Android APK using `expo build:android` (Note: You might need to make adjustments based on your environment and Firebase setup).

**To fix the error:** Refer to the code in `bugSolution.js` and ensure that you have a valid and correctly configured `google-services.json` file for your app's Firebase project in the correct directory.