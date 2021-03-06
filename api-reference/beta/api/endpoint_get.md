# Get endpoint

Retrieve the properties and relationships of a specific [endpoint](../resources/endpoint.md) object.

### Prerequisites
The following **scopes** are required to execute this API: *Group.Read.All* or *Group.ReadWrite.All*

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/endpoints/{id}
```
### Optional query parameters
This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.

### Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer &lt;token&gt; Required.|
| Content-Type   | Application/Json |

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [Endpoint](../resources/endpoint.md) object in the response body.
### Example
##### Request

<!-- {
  "blockType": "request",
  "name": "get_endpoint"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/endpoints/{id}
```
##### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Endpoint"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 208

{
  "capability": "Conversations",
  "providerId": "{Yammer GUID}",
  "providerName": "Yammer",
  "uri": "uri-value",
  "providerResourceId": "Yammer.FeedURL",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Endpoint",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->