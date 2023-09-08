# Image_Search_App
# Hosted Link:-https://tulasidurga1.github.io/Image_Search_App/
### This HTML and JavaScript code sets up a simple web page for performing image searches using the Unsplash API. Let's break down the code and explain how it works:

### HTML Structure:

- The HTML document is defined with the usual <!DOCTYPE html> declaration, specifying the document type as HTML5.
- The document's language is set to English using the <html lang="en"> tag.
- The <head> section contains metadata about the document, including character encoding, compatibility settings, viewport configuration, and the page title.
- An external CSS stylesheet (style.css) is linked to the document to apply styles to the content.
- The <body> section contains the main content of the webpage.
- HTML Elements:

-   <h1>: This element displays the page's main heading, which is "Image Search."

  - <form>: This is a form element used for user input. It contains:

- <input>: A text input field with the id "search-input" for entering search queries.
- <button>: A button with the id "search-button" for submitting the search query.
- <div class="search-results">: This empty div element with the class "search-results" will be used to display search results.

- <button id="show-more-button">Show more</button>: This button with the id "show-more-button" is initially hidden and will be used to load more search results.

### JavaScript:

- The JavaScript code starts by defining a variable accessKey, which holds an API access key for the Unsplash API. This key is used to authenticate requests to the API.

- It then selects various HTML elements using document.querySelector and getElementById to interact with them in JavaScript:

- form: The form element.
- searchInput: The search input field.
- searchResults: The container for displaying search results.
- showMoreButton: The button for loading more results.
- Two variables, inputData and page, are declared to store the user's search query and the current page number of results, respectively. inputData is initialized as an empty string, and page is initially set to 1.

### The searchImages function is defined as an asynchronous function. This function is responsible for fetching and displaying search results from the Unsplash API:

- It extracts the user's input from the search input field.
- Constructs a URL for the API request using the input data and the access key.
- Fetches data from the API using the fetch function and processes the JSON response.
- Clears the search results container when performing a new search (page === 1).
- Creates HTML elements for each search result (images and links) and appends them to the search results container.
- Increments the page variable for pagination.
- Displays the "Show more" button when there are more than one page of results.
### Event listeners are set up to handle user interactions:

- The submit event of the form is intercepted, preventing the default form submission behavior. Instead, the searchImages function is called to initiate the search.
- Clicking the "Show more" button triggers the searchImages function to load more results.
- Overall, this code creates a simple web page for searching and displaying images from Unsplash, providing a basic user interface for entering queries and viewing results with pagination.




