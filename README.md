# Project React Pure AF

This project contains a simple web page created using React. It demonstrates the basic steps to define a React component and render it in the DOM. Below is a detailed explanation of each part of the code.

## File Structure

The web page consists of a single HTML file structured as follows:

- `<!DOCTYPE html>`: Defines the document type and HTML version.
- `<html lang="en">`: The root element of the HTML document, `lang="en"` specifies that the content is in English.
- `<head>`: Contains metadata and links to external resources.
  - `<meta charset="UTF-8" />`: Sets the character encoding to UTF-8.
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`: Enables responsive web design, ensuring the web page looks good on various devices.
  - `<title>Pure React</title>`: Sets the title of the web page.
- `<body>`: Contains the visible content of the web page.
  - `<div id="root">not rendered</div>`: A container where the React component is rendered. The text "not rendered" acts as a placeholder and is replaced by React content.
  - `<script src="...">`: Includes external JavaScript files. In this case, React and ReactDOM libraries are included.
  - `<script>`: Defines JavaScript code directly in the HTML document.

## React Component

Within the `<script>` tag, a simple React component is defined and rendered:

1. **Component Definition:**

   - `const App = () => { ... }`: Defines a functional component `App`.
   - `React.createElement(...)`: Creates React elements. Here, a `div` element is created with an `h1` element as a child, containing the text "Hello World".

2. **Rendering:**
   - `const container = document.getElementById("root")`: References the container where the React component will be rendered.
   - `const root = ReactDOM.createRoot(container)`: Creates a root React element in the container.
   - `root.render(React.createElement(App))`: Renders the `App` component in the root element.

## Usage

To use the project, you can simply open the HTML file in a web browser. React will render the `App` component inside the `div` with the ID `root`, replacing the placeholder text "not rendered" with the output of the component, in this case, a `div` with an `h1` element that contains "Hello World".

## Notes

- The React files used are development versions and not suitable for production. For production environments, you should use the minified versions.
- This example doesn't use build tools or modules, which are recommended for more complex projects.

That's the basic structure and functionality of the web page. If you have any questions or need further information, feel free to ask!
