# Error codes v1

This is the universal error tracking system that the whole system uses.

*values in italic are unused*

| #   | HTTP code | Description                                                                                            |
| :-: |:---------:| ------------------------------------------------------------------------------------------------------ |
| 1   |    500    | General error, if you see this please create a ticket |
| 2   |    400    | Invalid data sent |
| 3   |    500    | Database error, if it persists please create a ticket |
| 5   |    400    | Invalid file format |
| 6   |    405    | Invalid method |
| 7   |    400    | String not trimmed |
| 8   |    400    | Request parameter missing |
| 10  |    400    | General error authentication error, if you see this please create a ticket |
| 11  |    403    | You don't have permission to do that |
| 12  |    401    | Incorrect password |
| 13  |    401    | Account is locked |
| 14  |    401    | Account is disabled |
| 15  |    401    | Account is expired |
| 16  |    404    | Unknown permission |
| 17  |    401    | Invalid authentication request |
| 18  |    401    | Invalid token |
| 19  |    429    | Too many requests |
| *20*|   *429*   | *Recaptcha error* |
| 21  |    401    | Invalid refresh token |
| 22  |    400    | Invalid grant type |
| 23  |    401    | Invalid authentication token *internal* |
| 24  |    503    | Auth service unavailable |
| 25  |    400    | External service (Google OpenID, Facebook access) token invalid |
| 26  |    400    | [Facebook account does not have email address associated](/documentation/loginandregister?id=warning) |
| 30  |    500    | General User error, if you see this please create a ticket |
| 31  |    404    | User not found |
| 32  |    409    | Username is already taken |
| 33  |    409    | Email address is already taken |
| 34  |    400    | [Registering with email address is disabled](/documentation/loginandregister?id=registration) |
| 35  |    400    | Consent is required to register |
| 36  |    400    | Invalid display name |
| 37  |    409    | External token already in use |
| 38  |    400    | You can't remove all forms of login |
| 50  |    500    | General group error, if you see this please create a ticket |
| 51  |    404    | Group not found |
| *52*|   *409*   | *Group name is already taken* |
| 53  |    400    | You cannot join that group |
| *54*|   *400*   | *You cannot invite into this group* |
| 55  |    400    | User already in group |
| 56  |    406    | Group password was invalid |
| 57  |    400    | User is not in the group |
| *58*|   *400*   | *Password is required for password protected group* |
| 59  |    400    | [Group limit reached](/documentation/limits) |
| 60  |    400    | [Invalid group type](/documentation/groups) |
| 61  |    404    | Invitation link not found |
| 70  |    500    | General task error, if you see this please create a ticket |
| 71  |    404    | Task not found |
| 72  |    400    | Task due date is invalid |
| 73  |    400    | [Task limit reached](/documentation/limits) |
| 90  |    500    | General comment error, if you see this please create a ticket |
| 91  |   *404*   | *Comment section not found* |
| 92  |    404    | Comment not found |
| 93  |    409    | User has already commented |
| *94*|   *401*   | *User is not owner of that comment* |
| 110 |    500    | General subject error, if you see this please create a ticket |
| 111 |    404    | Subject not found |
| 112 |    400    | [Subject limit reached](/documentation/limits) |
| 120 |    500    | General profile picture error, if you see this please create a ticket |
| 121 |    400    | Invalid size for profile picture |
| 122 |    400    | Invalid format for profile picture |
| 130 |    500    | General thera error, if you see this please create a ticket |
| 131 |    400    | Authentication request declined |
| 132 |    404    | Thera session not found |
| 133 |    409    | This session already exists |
| 134 |    400    | The sent URL is invalid |
| 135 |    400    | Invalid week number, must be between 1-53 |
| 136 |    400    | The session must be active to do that |
| 137 |    503    | Thera service currently unavailable |
| 138 |    503    | External service currently unavailable |
| 139 |    400    | [Thera session limit reached](/documentation/limits) |
| 170 |    503    | Hazizz service currently unavailable |