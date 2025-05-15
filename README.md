# CS50W Project 1 - Wiki

A Wikipedia-like online encyclopedia. This was Project 1 of HarvardX's [CS50W](https://www.edx.org/course/cs50s-web-programming-with-python-and-javascript) course in 2021 and was built using Python, Django, CSS, HTML, and Bootstrap.

## YouTube Video

Here is a short video where I walk through the project requirements and demonstrate the functionality as part of my course submission:  
[Watch the video](https://youtu.be/i0oxzX7iHIU?si=7uPuEyUZghrFWrcu)

## Specification

This project was built according to the following [specification](https://cs50.harvard.edu/web/2020/projects/1/wiki/):

- **Entry Page:** Visiting `/wiki/TITLE`, where `TITLE` is the title of an encyclopedia entry, displays the contents of that entry.
    - The view fetches the entry content using the appropriate `util` function.
    - If the requested entry does not exist, an error page informs the user that the page was not found.
    - If the entry exists, the page displays its content with the entry’s title.
- **Index Page:** The `index.html` lists all encyclopedia entries with clickable links that navigate directly to each entry’s page.
- **Search:** Users can search for encyclopedia entries using a search box in the sidebar.
    - If a query matches an entry’s title exactly, the user is redirected to that entry’s page.
    - If no exact match exists, a search results page shows all entries containing the query substring.
    - Users can click any result to view that entry.
- **New Page:** Clicking “Create New Page” in the sidebar allows users to add a new encyclopedia entry.
    - Users enter a title and Markdown content in a form.
    - Attempting to save a page with a duplicate title results in an error.
    - Otherwise, the entry is saved and the user is redirected to the new page.
- **Edit Page:** Each entry page includes a link to edit the Markdown content.
    - The edit page’s `textarea` is pre-filled with the current Markdown.
    - Users can save changes, which updates the entry and redirects back to its page.
- **Random Page:** Clicking “Random Page” loads a randomly selected encyclopedia entry.
- **Markdown to HTML Conversion:** Entry Markdown content is converted to HTML for display using the `python-markdown2` package (install via `pip3 install markdown2`).
    - For an additional challenge, implement Markdown to HTML conversion without external libraries, supporting headings, bold text, lists, links, and paragraphs.

