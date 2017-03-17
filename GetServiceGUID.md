## How to get a Service GUID using the CF API

This uses the Secure Gateway service as an example.

**GET**
  `https://api.ng.bluemix.net/v2/services?q=label:SecureGateway`

**Headers**
  * Key: `Authorization`
    * Value: `bearer <your bearer token>`


Response will include guid of the Secure Gateway service in the resources array under the "metadata" key

```
{
  "total_results": 1,
  "total_pages": 1,
  "prev_url": null,
  "next_url": null,
  "resources": [
    {
      "metadata": {
        "guid": "a132a5a9-4eb3-4b8d-bb43-3248b4badf5e",
        "url": "/v2/services/a132a5a9-4eb3-4b8d-bb43-3248b4badf5e",
        "created_at": "2015-02-16T01:48:40Z",
        "updated_at": "2017-03-17T01:35:53Z"
      },
```
