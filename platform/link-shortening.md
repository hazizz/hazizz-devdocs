# Dynamic links

## Firebase Dynamic links

Hazizz uses [Firebase Dynamic Links](https://firebase.google.com/docs/dynamic-links) to create share links.

Currently supported links:
* Group invite links

## Link shortener

These links tends to be long, therefore we created endpoints to shorten these links. These endpoints are part of the gateway module, they can be used without authentication, and they return a 308 response with a Location header.

Please refer to API documentation for further information.