# Expo CLI Android Build: 'gradlew' command not found

This repository demonstrates a bug in the Expo CLI's Android build process where the `gradlew` command is not found, despite Gradle being correctly installed.

## Bug Description
The Expo CLI fails to build the Android APK with an error indicating that `gradlew` is missing. This issue occurs inconsistently and is likely tied to environment variable management within the Expo CLI or its interaction with the Android build system.

## Reproduction Steps
1. Clone this repository.
2. Run `expo start`. 
3. Try building the Android APK using `expo build:android`. Observe that the build fails, reporting that `gradlew` is not found.

## Solution
The solution involves ensuring correct path configuration of Gradle within the Expo CLI's build process.  The provided `bugSolution.gradle` file offers a workaround that might resolve this issue in some cases.

## Additional Notes
This bug might be related to specific system configurations or Expo CLI versions.  Further investigation may be needed to pinpoint the root cause and find a more robust solution.