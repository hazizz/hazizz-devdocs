# Limitations

For better overall user experience and sustainability we placed limitations in the software.

## Rate limiting

The use of our API is limited by the following factors:
* You are able to send a request every 2 seconds in sustained manners
* You might send up to 10 requests in a burst manner
* If you are being rate limited we prove a [Retry-After header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After)

## Resource limiting

There is a limit how much resource a single user or group can use before hitting a limit.

#### Maximum groups
40 / User

#### Maximum tasks
150 / Owner (Group or user)

#### Maximum subjects
50 / Group

#### Maximum thera sessions
Unlimited unique accounts