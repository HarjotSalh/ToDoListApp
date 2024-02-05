# System Specifications

- **Device Name**: Salh
- **Processor**: 11th Gen Intel(R) Core(TM) i7-1195G7 @ 2.90GHz, 1.80 GHz
- **Installed RAM**: 16.0 GB (15.8 GB usable)
- **Device ID**: E0431910-C206-44D1-9D0E-45035AE8A0FE
- **Product ID**: 00342-21928-85103-AAOEM
- **System Type**: 64-bit operating system, x64-based processor
- **Pen and Touch**: Pen and touch support with 10 touch points

## Development Environment Setup

### Android Studio and SDK Installation

1. **Install Android Studio**:
   - Download from the [official download page](https://developer.android.com/studio).
   - Ensure the installation of Android SDK, SDK Platform, Android Virtual Device, and Performance (Intel ® HAXM) for emulator acceleration.

2. **Configure Android Studio**:
   - Open Android Studio to complete the initial setup wizard for the latest Android SDK.

### Node.js and npm Installation

1. **Download Node.js**:
   - Visit [Node.js website](https://nodejs.org/) and select the LTS version (64-bit Windows Installer).

2. **Install Node.js**:
   - Run the installer and follow the prompts with default settings.

3. **Verify Installation**:
   - In a command prompt, type `node -v` and `npm -v`.

### Java Development Kit (JDK)

1. **Download JDK 17**:
   - Go to [Oracle JDK 17 archive page](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html) and download the Windows x64 installer.

2. **Install JDK 17**:
   - Execute the installer with default settings.

3. **Configure Environment Variables**:
   - Set `JAVA_HOME` to your JDK path.
   - Ensure `ANDROID_HOME` is set to the Android SDK location.
   - Add the SDK's platform-tools to the system Path.

## Running on Device (Android)

### Enable USB Debugging

1. Activate "Developer options" by going to Settings → About phone and tapping Build number seven times.
2. Enable "USB debugging" in Developer options.

### Connect Device and Run App

1. Connect the device via USB and verify with `adb devices`.
2. Run `npm run android` in your project root.

### Connecting to Development Server

- **Via USB**: Use `adb reverse tcp:8081 tcp:8081`.
- **Via Wi-Fi**: Set the development machine's IP in the app's Dev Settings.

## Creating a React Native Project

1. **Project Initialization**: `npx react-native@latest init ProjectName`.
2. **Running the Project**: Start with `npm start`. For Android, use `npm run android`.
