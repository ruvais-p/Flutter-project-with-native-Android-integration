# Flutter ↔ Native Android Communication Example

This project demonstrates how to communicate between Flutter and native Android code using `MethodChannel`.

## ✨ Features

- Input your name in the Flutter app.
- Tap the button to send the name to native Android code.
- Native Android displays the name using a `Toast`.
- The same name is returned and displayed in the Flutter UI.

---

## 🛠️ Tech Stack

- **Flutter (Dart)**
- **Native Android (Kotlin)**
- `MethodChannel` for platform communication

---

## 📱 Flutter Code Overview

File: `homepage.dart`

### Widgets & Logic

- `TextField` for name input
- `MaterialButton` triggers native method call
- `MethodChannel` sends `"userName"` method call with a `Map<String, String>` parameter
- Native Android handles and returns the result
- Result is displayed on screen

---

## 🤖 Android Native Code Overview

File: `MainActivity.kt`

- Channel Name: `uniqueChannel`
- Listens for method `"userName"`
- Reads the argument `"name"`
- Displays it using a `Toast`
- Sends the name back to Flutter

---

## 🚀 How to Run

### Prerequisites

- Flutter installed
- Android Studio / emulator or real device

### Steps

1. Clone the repository or copy code to your project.
2. Run `flutter pub get`.
3. Connect an Android device or emulator.
4. Run the app using:

   ```bash
   flutter run
