# SMU-PCMOB6: Notes App

This is a React Native Notes app that includes user authentication and profile management. The app connects to a backend API for handling login and user information, and it uses React Navigation for managing different screens.

## Features

- **User Authentication**: Secure login with token storage using AsyncStorage.
- **Profile Management**: Display user profile information and allow user logout.
- **Loading Screen**: Show a loading indicator while the app checks authentication status.

## Technologies

- **React Native**: Framework for building native mobile applications.
- **React Navigation**: Navigation library for React Native.
- **AsyncStorage**: Storage system for persisting user tokens.
- **Axios**: HTTP client for making API requests.

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/smu-pcmob5-notes.git
    ```

2. **Navigate to the Project Directory**

    ```bash
    cd smu-pcmob5-notes
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

## File Structure

- `App.js`: Main entry point, handles navigation and authentication state.
- `screens/LoginScreen.js`: Manages user login and authentication.
- `screens/ProfileScreen.js`: Displays user profile and handles logout.
- `constants.js`: Contains screen names used in navigation.

## Contributing

To contribute to this project, please fork the repository and submit a pull request with your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

