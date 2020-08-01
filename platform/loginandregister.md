# Login and registration guideline

## Motivation
The Hazizz platform uses social logins for registration, and only provides limited native login features. The reason for this decision is that the selected services provide better user experience when it comes to handling lost accounts and forgotten passwords. This leads to a better user experience and a generally simpler login/register procedure.

## Login

### Account determination

When requesting a login, based on the email address you provide through your token you might get logged into an account, when you haven't registered with that social provider. This is a trust based system where if your verified email address matches you can log into your already existing account. 

### Ways to log in

#### Native login with username and password

This option only becomes available after registering an account and adding a password to it.

**This login is highly not advised**.

#### Refresh token

If the user has already authenticated before and you are in applicable time span you can use a refresh token.

#### Google OpenID
To validate these tokens we are using the Google [Google API Client](https://developers.google.com/identity/sign-in/web/backend-auth#using-a-google-api-client-library) with the following settings:

##### Issuers:
- https://accounts.google.com
- accounts.google.com
 
##### ClientIds:
- 425675787763-flqjv0n2nlcublglnonf795oul80feeg.apps.googleusercontent.com
- 425675787763-751dukg0oookea8tltaeboudlg0g555q.apps.googleusercontent.com

If you want to see your clientId on the list please contact us.

#### Facebook Login
To validate these tokens we are using the [Facebook Graph](https://graph.facebook.com/v4.0/) API, where we ask for the user's email address.

##### Warning
If the facebook address doesn't have an attached email address this throws an ErrorCode

## Registration

Registering a new account is only possible with either a Google or Facebook token.

The recommended way to handle registration for a better user experience is to not have a seperated login and register, rather only have login buttons, and if the server responds that the user is non-existant create a registration prompt.

When registering a user you must show our [Terms of Service](https://hazizz.hu/tos-en.txt) and our [Data policy](https://hazizz.hu/privacy-en.txt).