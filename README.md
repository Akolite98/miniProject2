# URL Formatter - Mini Project 2

This mini-project is a simple HTML file that takes a URL input from the user and formats it as a clickable link. It showcases the usage of JavaScript to validate and format URLs.

## Getting Started

To use this URL formatter, open the provided HTML file named `index.html` in your web browser. No additional setup or installation is required.

## How to Use

1. Open the `index.html` file in your web browser.

2. The web page will display a paragraph with the text "This is the link:" followed by an empty `<span>` element with the ID `link`.

3. The JavaScript code is embedded within the `<script>` tag after the `<p>` element.

4. The JavaScript code prompts the user to enter a URL using the `prompt()` function.

5. The code then checks if the URL starts with "http" (ignoring case) using `url.substr(0, 4) == "http"`. If it does, it logs "Its good already" to the browser console. If not, it prepends "http://" to the URL.

6. The code then creates an HTML anchor `<a>` tag with the user-provided or modified URL and sets it as the content of the `<span>` element using the `innerHTML` property.

7. The formatted URL will be displayed as a clickable link on the web page.

## Code Details

The implementation uses HTML and JavaScript to validate and format the user-provided URL.

### JavaScript Logic

The JavaScript code inside the `<script>` tag takes the user input for the URL using `prompt()` and stores it in the `url` variable.

It checks if the URL starts with "http" (ignoring case) using `url.substr(0, 4) == "http"`. If true, it logs "Its good already" to the browser console. Otherwise, it modifies the `url` variable by prepending "http://" to it.

Then, it selects the `<span>` element with the ID `link` using `document.getElementById("link")`. It creates an HTML anchor `<a>` tag with the user-provided or modified URL using string concatenation.

Finally, it sets the generated HTML code as the content of the `<span>` element, resulting in the formatted URL displayed as a clickable link.
