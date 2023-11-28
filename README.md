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
