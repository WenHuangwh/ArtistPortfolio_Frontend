# ArtistPortfolio_Frontend

## Setup and Installation

### Installing React
1. Verify the installation by running `node -v` and `npm -v` in the terminal.
    - Node version: v16.20.2
    - NPM version: 8.8.0.
2. If you don't have them installed, install Node.js and npm from the [Node.js official website](https://nodejs.org/).
3. Create a new React project using `npx create-react-app my-app`.
4. Navigate to the project directory (`cd my-app`).
5. Start the development server with `npm start`.

### Troubleshooting

#### Dependency Issue with babel-preset-react-app
- **Problem**: Missing dependency `@babel/plugin-proposal-private-property-in-object`.
- **Solution**: Run `npm install @babel/plugin-proposal-private-property-in-object --save-dev` to add it to `devDependencies`.


### Installing Tailwind CSS with Headless UI and Ant Design

#### Tailwind CSS Installation
1. `cd ap-app`
2. Install Tailwind CSS and its dependencies:
   ```bash
   npm install tailwindcss postcss autoprefixer
3. Create Tailwind configuration files:`npx tailwindcss init -p` This will create tailwind.config.js and postcss.config.js files in your project.
4. Configure Tailwind to Remove Unused Styles in Production:
   Edit `tailwind.config.js` to include the paths to all of your components so Tailwind can tree-shake unused styles in production builds:
   ```bash
   module.exports = {
     content: [
       "./src/**/*.{js,jsx,ts,tsx}",
       // more files or globs
     ],
     // ...
   };
5. Include Tailwind in Your CSS:
   In your src/index.css or src/styles.css, include the Tailwind directives:
   ```bash
   @tailwind base;
   @tailwind components;
   @tailwind utilities;

#### Install Headless UI
Headless UI provides completely unstyled, fully accessible UI components, designed to integrate beautifully with Tailwind CSS.
1. Install Headless UI via npm: `npm install @headlessui/react`
2. Use Headless UI Components:
   You can now use components from Headless UI in your project. Import them in your React components like so:
   ```bash
   import { Dialog, Transition } from '@headlessui/react';
   
  
#### Install Ant Design
1. `npm install antd --save`
2. Usage: We strongly discourage loading the entire files this will add bloat to your application and make it more difficult to receive bugfixes and updates. Antd is intended to be used in conjunction with a build tool, such as webpack, which will make it easy to import only the parts of antd that you are using.

   ```bash
   import React from 'react';
   import { DatePicker } from 'antd';
   
   const App = () => {
   return <DatePicker />;
   };
   
   export default App;

