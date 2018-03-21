## Runing Swagger UI

* Clone the repo swagger-ui in your local machine
* Update the file “dist\index.html” by replacing the text “<<Add_ClientSecret_here>>” with the client secret that is used to protect the API specs
* Host the contents of the “dist” folder in your localhost webserver (any static file sever such as Nginx or IIS will do)
* Browse the hosted “index.html” page
* Enter the URL of the API specs (example, https://api.cxaoneuat1.com/hrapi/docs/v1/specs.json for HR Portal API specs) to see the API specifications in a readable form

## How to test out an API?

* To test out a protected API, get the “session token” or the “access token” after logging in
* Click the “Authorize” button in the top right part of the “index.html” page
* Type in “Bearer {{access_token}}” filling in the access token in the placeholder
* Expand the API you want to try out and click “Try it out”
* Specify any input params if the API requires and / or click “Execute”
* The response from the API will be shown once it's obtained

## Note
* The API specs will only be available in Dev / Test environments
* To keep the API specs secure (even in Dev / Test env), you need a client secret (which can be the same across different API backends) that will be available to all Developers
