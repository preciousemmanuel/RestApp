# Mobile Application

This is a React Native mobile application built with TypeScript, featuring a modern, scalable architecture.

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or later)
- Watchman (recommended for macOS)
- Xcode (for iOS development)
- Android Studio (for Android development)
- React Native CLI

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Add Custom Fonts:**
    This project is configured to use the Roboto font family. To add the font files:
    - Download Roboto from [Google Fonts](https://fonts.google.com/specimen/Roboto).
    - Place the `.ttf` files (e.g., `Roboto-Regular.ttf`, `Roboto-Bold.ttf`) into the `/assets/fonts/` directory.
    - Link the font assets by running:
      ```bash
      npx react-native-asset
      ```

### Running the Application

- **For iOS:**
  ```bash
  npm run ios
For Android:
npm run android
🏗️ Architecture
This project follows a modern, scalable architecture for React Native development.

Core Libraries
React Navigation: For handling all navigation logic, including the root authentication flow, a main stack, and a bottom tab navigator.
Redux Toolkit: For global state management. We use it for:
RTK Query: For efficient data fetching, caching, and managing server state (/src/services/api.ts).
authSlice: For managing the user's authentication token and status.
themeSlice: For managing the application's theme (light/dark/system).
TypeScript: For static typing and improved developer experience.
Project Structure
src/components: Contains reusable components used throughout the application (e.g., Button, Container, Header).
src/hooks: Custom hooks, such as useTheme.
src/navigation: All navigation-related code, including stacks and tab navigators. The RootNavigator handles the switch between authenticated and unauthenticated flows.
src/screens: Feature-based screen components.
src/services: API service definitions using RTK Query.
src/store: Redux store configuration and slice definitions.
src/styles: Global and component-specific style definitions.
src/theme: Theme-related files, including color palettes and metrics.
src/types: TypeScript type definitions for the application.
Styling
The application uses a custom theme system built on top of React Native's StyleSheet. A useTheme hook provides access to theme-aware colors, which allows for easy implementation of light and dark modes.

✅ Running Tests
The project uses Jest for testing. To run the test suite, use the following command:

npm test
