Get your Bluemix bearer token

POST
  `https://login.ng.bluemix.net/UAALoginServerWAR/oauth/token`

Headers
  key: `Authorization`
  value: `Basic Y2Y6`

  key: `Accept`
  value: `application/json`

Body
  key: `grant_type`
  value: `password`

  key: `username`
  value: `<your bluemix username>`
  
  key: `password`
  value: `<your bluemix password>`

Response will include an "access_token" this is your bearer token copy this and use
for the Authorization header in the next call.

Example
```
{
  "access_token": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "expires_in": 1209599,
  "scope": "openid mccp_stealth_visibility.all uaa.user cloud_controller.read password.write cloud_controller.write",
  "jti": "xxxxxxxxxxxxxxxxxxxxxx"
  ```