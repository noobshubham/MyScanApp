# MyScanApp

MyScanApp is an Android application that allows users to scan a product using their device's camera, process the image with Google Gemini Pro, and store the processed data in Firebase Firestore.

## Features

- Scan product using CameraX
- Send the scanned image to Google Gemini Pro for processing
- Store the response JSON from Google Gemini Pro in Firebase Firestore

## JSON File Requirements

The JSON response from Google Gemini Pro should contain the following fields:
- `Product Name`
- `Description`
- `Colour`
- `Pattern`

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Android Studio 4.1 or later
- Firebase Account
- Google Gemini Pro API access

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/noobshubham/MyScanApp.git
   cd MyScanApp
   ```
2. **Open the project in Android Studio:**
   - Start Android Studio and select `Open an existing Android Studio project`.
   - Navigate to the cloned directory and select it.

3. **Configure Firebase:**
   - Go to the [Firebase Console](https://console.firebase.google.com/).
   - Create a new project or use an existing one.
   - Add an Android app to your Firebase project with your app's package name.
   - Download the `google-services.json` file and place it in the `app` directory of your project.
   - Add Firebase SDK to your project by following the instructions in the Firebase console.

4. **Add Google Gemini Pro API Key:**
   - Create a file named `apikeys.properties` in the root directory of your project.
   - Add your Google Gemini Pro API key:
    ```makefile
    GEMINI_PRO_API_KEY=your_api_key_here
    ```

5. **Build and run the project:**
   - Sync the project with Gradle files.
   - Run the app on an emulator or a physical device.

### Usage

1. Open the app on your device.
2. Tap the "Scan Product" button to open the camera.
3. Capture the image of the product you want to scan.
4. The app will send the image to Google Gemini Pro for processing.
5. The processed data will be saved in Firebase Firestore.

### License
This project is licensed under the MIT License - see the LICENSE file for details.

### Acknowledgments

- [CameraX](https://developer.android.com/training/camerax)
- [Firebase](https://firebase.google.com/)
- [Google Gemini Pro](https://ai.google.dev/)

### Contact
For any questions or suggestions, please reach out to me at contact@noobshubham.eu.org.