## Get your Bluemix bearer token

**POST**
  `https://login.ng.bluemix.net/UAALoginServerWAR/oauth/token`

**Headers**
  * Key: `Authorization`
    * Value: `Basic Y2Y6`

  * Key: `Accept`
    * Value: `application/json`

**Body**
  * Key: `grant_type`
    * Value: `password`

  * Key: `username`
    * Value: `<your bluemix username>`
  
  * Key: `password`
    * Value: `<your bluemix password>`

The response will include an `access_token` this is your bearer token.

Example
```
{
  "access_token": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "expires_in": 1209599,
  "scope": "openid mccp_stealth_visibility.all uaa.user cloud_controller.read password.write cloud_controller.write",
  "jti": "xxxxxxxxxxxxxxxxxxxxxx"
  ```
