
# Chat-App with React-Native and Firebase

This project is a real-time chat application built using React Native for the front-end and Firebase for the backend. The application allows users to send and receive messages in real-time, providing a seamless chat experience across devices.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Installation](#installation)
  - [Step 1: Clone the Repository](#step-1-clone-the-repository)
  - [Step 2: Install Required Libraries](#step-2-install-required-libraries)
  - [Step 3: Install Navigation and Additional Dependencies](#step-3-install-navigation-and-additional-dependencies)
  - [Step 4: Set Up Firebase](#step-4-set-up-firebase)
- [Usage](#usage)
  - [Running the Application](#running-the-application)
  - [Firebase Authentication](#firebase-authentication)
  - [Real-time Chat](#real-time-chat)
- [Explanation](#explanation)
  - [Components](#components)
  - [Navigation](#navigation)
  - [Screens](#screens)
- [Deployment](#deployment)
  - [Push Your Project to GitHub](#push-your-project-to-github)
- [Authors](#authors)
## Overview
This Chat App allows users to communicate in real-time using Firebase as the backend service. The application supports user authentication, real-time messaging, and more, optimized for both Android and iOS devices.
## Features
- **Real-time Messaging:** Send and receive messages instantly using Firebase's Firestore.
- **User Authentication:** Secure authentication using Firebase Authentication (Email/Password).
- **User Profiles:** Manage user profiles.
- **Responsive Design:** Optimized for both Android and iOS devices.
- **Navigation:** Smooth navigation between screens using React Navigation.
- **Persistent Login:** Users remain logged in using AsyncStorage, even after closing the app.

## Tech Stack

- **Front-end:** React Native
- **Back-end:** Firebase (Authentication, Firestore)
- **Languages:** JavaScript
- **Deployment:** Android/iOS
## Requirements

The following dependencies are required:

- `@react-native-firebase/app`
- `@react-native-firebase/auth`
- `@react-native-firebase/firestore`
- `react-navigation`
- `react-native-vector-icons`
- `react-native-gesture-handler`
- `@react-navigation/native`
- `@react-navigation/stack`
- `react-native-screens`
- `react-native-safe-area-context`
- `react-native-uuid`
- `react-native-gifted-chat`

## Installation

### Step 1: Clone the Repository:

```bash
https://github.com/Lucky9451/Chat-App-with-React-Native.git
cd Chat-App-with-React-Native
```

### Step 2: Install Required Libraries

Install the necessary packages using npm:
```bash
npm install
```

### Step 3: Install Navigation and Additional Dependencies

To enable smooth navigation between screens and use UUIDs in your app, install the following packages:

- React Navigation:

```bash
npm install @react-navigation/native
```
- Screens and Safe Area Context:

```bash
npm install react-native-screens react-native-safe-area-context
```
- Gesture Handler:

```bash
npm install react-native-gesture-handler
```
- Navigation Stack:

```bash
npm install @react-navigation/stack
```
- UUID Generation:

```bash
npm install react-native-uuid
```
- Gifted Chat (for the chat interface):

```bash
npm install react-native-gifted-chat
```
### Step 4: Install Navigation and Additional Dependencies

- Create a new Firebase project on Firebase Console.
- Add an Android/iOS app to your Firebase project and follow the setup instructions.
- Download the google-services.json file for Android or GoogleService-Info.plist file for iOS, and place them in the appropriate directories (android/app/ for Android, ios/ for iOS).
- Enable Firebase Authentication and Firestore in your Firebase project.
## Usage

### Running the Application

Ensure that your development environment is set up for React Native (Android/iOS).

- Start the Metro bundler:

```bash
npx react-native start
```
- Run the application on your device/emulator:

```bash
npx react-native run-android  # for Android
npx react-native run-ios  # for iOS
```
### Firebase Authentication
- Sign up or log in using Firebase Authentication.
- Update your user profile with a display name and avatar.

### Real-time Chat
- Start a chat with another user.
- Send and receive messages in real-time.
- Receive push notifications for new messages.
## Explanation

### Components
- **Loader.js:** A loading spinner component used to indicate when an operation is in progress.
### Navigation
- **AppNavigator.js:** Manages the app's navigation flow using React Navigation.
### Screens
- **Signup.js:** Screen for user registration. Users can sign up by providing their name, email, mobile number, and password. Data is stored in Firebase.

- **Login.js:** Screen for user login. It checks credentials against Firebase and logs the user in, storing session data using AsyncStorage.

- **Chat.js:** The main chat interface where users can send and receive messages in real-time. Messages are stored in Firebase Firestore.

- **Splash.js:** The splash screen displayed when the app starts. It checks if the user is already logged in using AsyncStorage.

- **Main.js:** The main screen with a bottom tab navigation, allowing users to switch between different tabs such as Users and Settings.

### Usage
- Signup/Login: Users can sign up or log in using their credentials. The app will navigate to the Main screen upon successful login.
- Real-Time Chat: The Chat screen allows users to engage in real-time conversations. Messages are persisted in Firebase and retrieved on subsequent logins.
- Navigation: The app uses a stack-based navigation flow, starting with the Splash screen and moving to either the Login or Main screen based on user authentication status.
- AsyncStorage: The app stores user session data locally using AsyncStorage, ensuring that users remain logged in even after closing the app.
## Deployment

1. **Push your project to GitHub**:
    - Initialize a new Git repository if you haven't already:
      ```bash
      git init
      ```
    - Add your files to the repository:
      ```bash
      git add .
      ```
    - Commit your changes:
      ```bash
      git commit -m "Initial commit"
      ```
    - Create a new repository on GitHub.
    - Link your local repository to the GitHub repository:
      ```bash
      git remote add origin https://github.com/yourusername/Chat-App-with-React-Native.git
      ```
    






## Authors

- [Lucky Verma](https://github.com/Lucky9451)

