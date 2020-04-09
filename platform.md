 # Platform

To make this project work we are using multiple REST based services. To understand and use these services you can find documentations in this section.

## API
The API documentation can be found in the sidebar.

## Modules
The platform is made of multiple microservices. These services can be private or public based on whether a user can interact with them or not.

### Public

* **Gateway**

The gateway is responsible for transferring the requests between the modules and the outside world. It functions as tracking and security layer, with some added functionality.

* **Auth module**

This Auth module is responsible basic user management like authentication, authorization and account removal.

* **Házizz module** 

This module serves as the main module for the project. This contains and manages the tasks, the groups, and everything connected to them. 

* **Théra module**

Théra module is our integration service, that creates a bridge between the outside world and our platform. The use of this module allows us to deliver optimal user experience.

### Private

* [**Kreta proxy module**](https://github.com/hazizz/kreta-proxy) *open-source*

This is a proxy module for E-Kréta. This handles communication with their service and transformation of their data.

* **Notificator module** *preview*

This is a helper module that periodically check the users' state, and depending on them send a push to notification.

WIP

## Contact

If you have any feedback with the platform please reach out to us by any means described on [our website](https://hazizz.hu).

If you find any issues or problems with the service please open a ticket on [our platform repository](https://github.com/hazizz/hazizz-platform/issues).