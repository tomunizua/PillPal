# Medication Reminder App

This is a cross-platform medication reminder app built using React Native and Expo. The app allows users to add medications, schedule reminders, and view their medication history. The app also supports web notifications using Firebase Cloud Messaging (FCM).

## Features

- User registration and login
- Add, update, and delete medications
- Schedule notifications for medication reminders
- View medication history
- Web push notifications using FCM

## Prerequisites

- Node.js and npm installed
- Expo CLI installed (`npm install -g expo-cli`)
- Firebase project setup with Firestore and FCM

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/medication-reminder-app.git
    cd medication-reminder-app
    ```

2. Install dependencies:

    ```bash
    npm install
    ```

3. Configure Firebase:

    - Replace the Firebase configuration in `firebaseConfig.js` with your own Firebase project configuration.
    - Replace `YOUR_PUBLIC_VAPID_KEY_HERE` with your actual VAPID key in `AddMedicationScreen.js`.
    - Replace `YOUR_SERVER_KEY` with your actual FCM server key in `AddMedicationScreen.js`.

4. Run the app:

    - For iOS/Android:

        ```bash
        expo start
        ```

    - For web:

        ```bash
        npx expo export:web
        ```

## Firebase Configuration

Make sure to set up Firestore and FCM in your Firebase project:

1. Go to the Firebase console.
2. Create a new project or select an existing one.
3. Enable Firestore in the "Database" section.
4. Enable FCM in the "Cloud Messaging" section.
5. Generate and copy the VAPID key for web push notifications.
6. Get the server key from the FCM settings.

## Project Structure

- `App.js`: The main entry point of the app.
- `firebaseConfig.js`: Firebase configuration and initialization.
- `screens/`: Contains the different screens of the app (e.g., login, register, home, add medication, update medication, profile, history).
- `components/`: Contains reusable components.
- `assets/`: Contains static assets like images and fonts.
- `web-build/`: Contains the web build output (generated after running `npx expo export:web`).

## Dependencies

- React Native
- Expo
- Firebase
- React Native Paper
- React Navigation

## Troubleshooting

If you encounter any issues, please check the following:

- Ensure all dependencies are installed correctly.
- Ensure your Firebase configuration is correct.
- Check for any error messages in the console and debug accordingly.

## License

This project is licensed under the MIT License.
