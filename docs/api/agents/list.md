This method returns a list of Agent resources.

**URL**

`/agents`

**Method**

`GET`

**Parameters**

| Parameter Name | Type   | Value | Description
| ---  | :--------- |  :--------- |  :--------- |
| filter |  query | string | Use filter to narrow the elements shown. |

Note: The filter parameter uses [JsonPath](https://github.com/json-path/JsonPath) format

**Request body**

Do not supply a request body with this method.

**Response**

If successful this method returns a list of Agent resources.

**Sample Call**

```json
GET /api/v1beta1/agents
{

}

HTTP/1.1 200 OK
{
  "status": "200",
  "message": "Successful request",
  "result" : [{
      "apiVersion": "v1beta1",
      "kind": "Agent",
      "metadata": {
      	"name": "John Doe",
        "ref": "ag3f77f6"
      },
      "spec": {
      	"credentials": {
      		"username": "1001",
      		"secret": "1234"
      	},
      	"domains": [
      		"sip.local"
      	]
      }
  }]
}
```