# Bharat States Highlighter

## 1. Project Title and Description
This is a simple web application consisting of a single HTML page. Its purpose is to display a patriotic title, "I am really proud of my bharat," and a list of three Indian states. A key feature of this application is the integration of `highlight.js` to process and style the main title, demonstrating its usage within a `<code>` block, even for plain text.

## 2. Setup Instructions
This web application is extremely simple and does not require any complex setup or build process.

1.  **Save the file**: Save the `index.html` content provided into a file named `index.html` in a directory of your choice.
2.  **Open in browser**: Simply open the `index.html` file using any modern web browser (e.g., Chrome, Firefox, Edge, Safari). You can do this by double-clicking the file or dragging it into your browser window.

No server or external dependencies (beyond the CDN for `highlight.js`) are required.

## 3. Usage Guide
Upon opening `index.html` in your browser, you will see:

*   A prominent title, "I am really proud of my bharat," displayed at the top. This title is enclosed within a `<code>` block, and its rendering is influenced by the `highlight.js` library, which applies its default styling for plain text.
*   Below the title, there will be a section listing three popular Indian states: Maharashtra, Karnataka, and Rajasthan.

The page is static and interactive elements are not included beyond the initial rendering.

## 4. Code Explanation

*   **`index.html`**: This is the sole file in the project and contains the entire structure and logic for the web page.
    *   **HTML Structure**: It includes the basic HTML5 boilerplate, a `<head>` section with metadata and a `<title>` tag set to "I am really proud of my bharat" (for the browser tab).
    *   **`highlight.js` Integration**: 
        *   The `highlight.js` CSS stylesheet is linked from a CDN in the `<head>` section (`default.min.css`). This provides the styling for the highlighted code blocks.
        *   The main title "I am really proud of my bharat" is wrapped within an `<h1>` tag, which in turn contains `<pre><code class="language-plaintext">I am really proud of my bharat</code></pre>`. The `language-plaintext` class instructs `highlight.js` to treat the content as plain text, applying its default visual style for non-code elements.
        *   The `highlight.js` JavaScript library is linked from a CDN at the end of the `<body>` for optimal loading performance.
        *   A small inline `<script>` block is used to initialize `highlight.js` by calling `hljs.highlightAll()` once the DOM content is fully loaded. This function automatically finds all `<pre><code>` blocks on the page and applies the appropriate highlighting.
    *   **State Names**: Three separate `<p>` tags are used to display the names of the Indian states.
    *   **Custom CSS**: A `<style>` block is included in the `<head>` to provide basic styling for the body, headings, paragraphs, and a container for the highlighted title, enhancing the overall aesthetic of the page.

## 5. License Information
This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the terms of the license.
