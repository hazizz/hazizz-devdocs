2020.04.28:
- Openapi 3 and JSON Schema files are now available for developers.
- Added corresponding documentation pages. (Swagger documentation, and data structures)

2020.04.27:
- Data schemas revised, and endpoints have been sorted into categories. 
- Deprecations have been flagged.

2020.04.26:
- Springfox replaced with Springdoc-openapi. [Avaiable now](https://hazizz.duckdns.org:9000/swagger-ui.html) *Each module now does **not** have their own separate swagger-ui.*
- Json Schema generation for developer documentation in work (goal: code generation for clients)
- Spring boot and Spring cloud version upgrade
- CORS filter fixed*
- Started on documenting API in code. 1 down, 2 to go.

2020.04.10:
- Guide on rate limiting
- New rate limit implementation Guava -> Bucket4j
- Gateway now handles logging, rate limiting, and CORS separately.

`*` = Was live before this patch note.