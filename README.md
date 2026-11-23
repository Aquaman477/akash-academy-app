# Akash Academy Android App

Android wrapper for the Akash Academy coaching-class app. The interface is bundled inside the APK and works offline using browser-local storage.

## Build an APK using GitHub Actions

1. Create a new GitHub repository, for example `akash-academy-app`.
2. Extract this ZIP file.
3. Upload **all files and folders inside** `akash_academy_android` to the repository root. The `.github/workflows/build-apk.yml` file must remain in that exact path.
4. Commit the files to the `main` branch.
5. Open the repository on GitHub and select **Actions**.
6. Open **Build Akash Academy APK**. It will run automatically after the push. You can also choose **Run workflow**.
7. When the workflow finishes, open the successful run and download the artifact named `akash-academy-debug-apk`.
8. Extract the downloaded artifact. It contains `app-debug.apk`. Transfer it to your Android phone and install it. You may need to allow installation from that file manager/browser.

## Build locally in Android Studio

Open this folder in Android Studio, allow Gradle sync, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

## Current app capabilities

- Dashboard
- Study library: upload PDF, Word, PowerPoint and image files
- Question bank with grade, chapter, question type, marks and difficulty
- Test configuration and question selection from saved question bank
- Test preview and Android print-to-PDF flow
- Student list and result register
- JSON backup export/import

## Important limitations

This is a first Android APK prototype. Data is stored locally on the device/browser profile; it is not synchronised to the cloud. There is no secure teacher/student authentication, remote student access, online timed test delivery, server-side file storage, or AI extraction/generation yet. Do not use it as a multi-device student platform until a backend and authentication are added.

## App identity

- App label: Akash Academy
- Application ID: `com.akashacademy.app`
- Version: `1.0.0`
- Minimum Android: Android 6.0 (API 23)
