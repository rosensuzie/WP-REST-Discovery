# Wordpress REST API discovery with JavaScript (ES6)

The wordpress REST api has a built-in method that allow clients to find the WordPress REST API's entry point.
The way it works is by adding a `<link>` tag to the page with attribute `rel = "https://api.w.org/"` to the document source code.
The code here is a concise ES6 implementation of the code example from Wordpress docs here: https://developer.wordpress.org/rest-api/using-the-rest-api/discovery/#element

`const apiRoot = [...document.querySelectorAll('link')].filter(li=>li.rel === "https://api.w.org/")[0].href`
