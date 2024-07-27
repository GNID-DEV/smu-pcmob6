# SMU-PCMOB6: Notes App

This is a React Native Notes app that includes user authentication and profile management. The app connects to a backend API for handling login and user information, and it uses React Navigation for managing different screens.

## Features

- **Authentication**: Users can log in or register with email and password.
- **Notes Management**: Users can create, view, edit, and delete notes.
- **Profile Management**: Users can view and edit their profile information.
- **Camera Functionality**: Users can take photos using the device camera and save them.

## Technologies

- **React Native**: Framework for building the mobile app.
- **Redux Toolkit**: State management.
- **Firebase**: Backend for managing notes.
- **AsyncStorage**: Local storage for authentication tokens and photo URIs.
- **Expo**: Provides camera and vector icon functionalities.

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/gnid-dev/smu-pcmob6.git
    ```

2. **Navigate to the Project Directory**

    ```bash
    cd smu-pcmob6
    ```

3. **Install Dependencies**

    ```bash
    npm install
    ```

4. **Run the App**

    ```bash
    npm start
    ```

## Setup

1. **API Configuration**

    - Update the `API` and `API_LOGIN` constants in `LoginScreen.js` and `API_WHOAMI` in `ProfileScreen.js` with your backend API endpoints.

2. **AsyncStorage**

    - Ensure that `AsyncStorage` is properly set up for storing and retrieving user tokens.

## Project Structure

- **App.js**: Main entry point for the application.
- **components/**: Contains React components used throughout the app.
    - **HomeStack.js**: Bottom tab navigator for home screens.
    - **NotesStack.js**: Stack navigator for notes-related screens.
    - **ProfileStack.js**: Stack navigator for profile-related screens.
- **screens/**: Contains screen components for different app views.
    - **AuthScreen.js**: Login and registration screen.
    - **NotesScreenAdd.js**: Screen for adding a new note.
    - **NotesScreenHome.js**: Home screen for viewing notes.
    - **NotesScreenDetails.js**: Screen for viewing note details.
    - **ProfileScreen.js**: Profile screen.
    - **CameraScreen.js**: Screen for taking and saving photos.
- **store/**: Contains Redux store configuration and slices.
    - **notesSlice.js**: Manages the state for notes.
    - **firebase.js**: Firebase configuration and initialization.

## Constants
- constants.js: Contains constant values used across the app, such as API endpoints and route names.

## Usage

### Authentication

1. Navigate to the AuthScreen to log in or register a new account.
2. Use valid credentials to access the main features of the app.

### Notes Management
1. After logging in, navigate to the NotesStack to view, add, or manage your notes.
2. Use the NotesScreenAdd to create a new note.
3. View and edit notes on the NotesScreenDetails.

### Profile and Camera
1. Navigate to the ProfileStack to view and edit your profile.
2. Use the CameraScreen to take photos and save them to your profile.

## Contributing

To contribute to this project, please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

