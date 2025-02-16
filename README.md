# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh


# React Practice EP1

Welcome to **React_Practice_EP1**! This repository contains the basic React concepts I learned today, along with sample code snippets for each topic.

## Topics Covered

### 1. What is React?
React is a JavaScript library for building user interfaces. It allows developers to create reusable UI components and manage application state efficiently.

### 2. What is JSX?
JSX (JavaScript XML) is a syntax extension for JavaScript that allows writing HTML-like structures within JavaScript code. JSX makes React components more readable and expressive.

Example:
```jsx
const element = <h1>Hello, React!</h1>;
```

### 3. Setting Up the Local Environment
To start working with React locally, follow these steps:
1. Install Node.js and npm (Node Package Manager).
2. Create a new React project using Create React App:
   ```sh
   npx create-react-app my-app
   cd my-app
   npm start
   ```

### 4. Our First Component
React components are reusable UI elements. Here’s a simple functional component:
```jsx
function Greeting() {
  return <h1>Hello, World!</h1>;
}
export default Greeting;
```

### 5. Import and Export in React
Components are imported and exported to use them in different files.

Example:
```jsx
// Exporting a component
export default function Welcome() {
  return <h1>Welcome to React!</h1>;
}

// Importing the component
import Welcome from './Welcome';
```

### 6. Writing Markup in JSX
JSX allows embedding HTML-like structures inside JavaScript code.
```jsx
const element = <div>
  <h1>JSX Example</h1>
  <p>This is a paragraph inside a JSX element.</p>
</div>;
```

### 7. React Fragments
React Fragments allow grouping multiple elements without adding extra nodes to the DOM.
```jsx
import React from 'react';
function Example() {
  return (
    <>
      <h1>Heading</h1>
      <p>Paragraph inside a React Fragment.</p>
    </>
  );
}
export default Example;
```

### 8. JSX with Curly Braces
JSX allows embedding JavaScript expressions inside curly braces `{}`.
```jsx
const name = 'John';
const element = <h1>Hello, {name}!</h1>;
```

### 9. Structuring Components
Breaking UI into smaller components improves readability and reusability.
```jsx
function Header() {
  return <h1>My Website</h1>;
}

function App() {
  return (
    <div>
      <Header />
      <p>Welcome to my website.</p>
    </div>
  );
}
export default App;
```

### 10. Styling Components
There are multiple ways to style components in React:

- **Inline Styles**
```jsx
const styles = {
  color: 'blue',
  fontSize: '20px'
};

function StyledComponent() {
  return <p style={styles}>This is a styled paragraph.</p>;
}
```

- **CSS Modules**
```css
/* styles.module.css */
.title {
  color: red;
  font-size: 24px;
}
```
```jsx
import styles from './styles.module.css';

function StyledComponent() {
  return <h1 className={styles.title}>Styled with CSS Module</h1>;
}
```

---
## Getting Started
To clone and run this repository locally:
```sh
git clone https://github.com/your-username/React_Practice_EP1.git
cd React_Practice_EP1
npm install
npm start
```

## Conclusion
This repository is a starting point for understanding the basics of React. More advanced concepts will be added in future episodes.

Happy Coding! 🚀





