# LinkedIn Clone

A LinkedIn clone built with React and Vite, featuring a sign-in page and a home page layout with a navbar, left side, right side, and main components. Redux will be integrated to handle more complex interactions on posts.

## Features

- **Sign-In Page:** User authentication interface.
- **Home Page:** Layout includes navbar, left side, right side, and main content areas.
- **Upcoming:** Redux integration for handling interactions on posts.

## Getting Started

To get started with the project, follow these steps:

### Installation

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

### Development

To start the development server, run:
```bash
npm run dev
```

The application will be available at `http://localhost:3000`.

### Building for Production

To create a production build, use:
```bash
npm run build
```

### Project Structure

- **`node_modules/`**: Contains all the project dependencies.
- **`public/`**: Stores public assets like `index.html`.
- **`src/`**: Contains the application’s source code.
  - **`components/`**: Reusable React components.
    - **`Header.jsx`**: Navigation bar component.
    - **`Home.jsx`**: Main layout component.
    - **`Leftside.jsx`**: Left side component for home layout.
    - **`Login.jsx`**: Sign-in page component.
    - **`Main.jsx`**: Main area component for home layout.
    - **`Rightside.jsx`**: Right side component for home layout.
  - **`reducers/`**: Stores Redux reducers (currently under development).
  - **`store/`**: Contains the Redux store setup.
  - **`App.jsx`**: Main application component.
  - **`App.css`**: Global styles for the application.
  - **`index.jsx`**: Entry point for React application.
  - **`index.css`**: Additional global styles.
  - **`main.jsx`**: Renders the React app to the DOM.
- **`.gitignore`**: Specifies files to be ignored by Git.
- **`eslint.config.js`**: Configuration file for ESLint.
- **`index.html`**: Main HTML file in the public folder.
- **`package.json`**: Manages project dependencies and scripts.
- **`vite.config.js`**: Vite configuration file.

### Netlify Hosting and Routing

If you are hosting this project on Netlify, you'll need to configure a `_redirects` file to ensure proper routing for your single-page application (SPA).

#### Steps to Set Up:

1. In the `public/` directory, create a file named `_redirects` if it doesn't already exist.
   
2. Add the following line to the `_redirects` file:

   ```plaintext
   /*    /index.html   200
   ```

3. Redeploy the project to Netlify.

This setup ensures that all routes (e.g., `/home`, `/login`, `/profile`, etc.) will correctly load `index.html`, and React Router will manage the routing on the client-side.

### Redux Integration

Upcoming features will involve setting up Redux to manage state for post interactions and other complex functionalities. Detailed instructions will be provided as the implementation progresses.