##ReConnectionMethodType Enum
'ReConnectionMethodType enum. Encapsulates the object that represents reconnectionmethodtype in Go.'
## ReConnectionMethodType Enum
Specifies what the spreadsheet application should do when a connection fails.
```go
type ReConnectionMethodType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Required](./required/) | On refresh use the existing connection information and if it ends up being invalidthen get updated connection information, if available from the external connection file. |
|[Always](./always/) | On every refresh get updated connection information from the external connection file,if available, and use that instead of the existing connection information.In this case the data refresh will fail if the external connection file is unavailable. |
|[Never](./never/) | Never get updated connection information from the external connection fileeven if it is available and even if the existing connection information is invalid |
