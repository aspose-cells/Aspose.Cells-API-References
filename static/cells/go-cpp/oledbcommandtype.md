##OLEDBCommandType Enum
'OLEDBCommandType enum. Encapsulates the object that represents oledbcommandtype in Go.'
## OLEDBCommandType Enum
Specifies the OLE DB command type.
```go
type OLEDBCommandType int32
```
## Fields
| Field | Description |
| --- | --- |
|[None](./none/) | The command type is not specified. |
|[CubeName](./cubename/) | Specifies a cube name |
|[SqlStatement](./sqlstatement/) | Specifies a SQL statement |
|[TableName](./tablename/) | Specifies a table name |
|[DefaultInformation](./defaultinformation/) | Specifies that default information has been given, and it is up to the provider how to interpret. |
|[WebBasedList](./webbasedlist/) | Specifies a query which is against a web based List Data Provider. |
|[TableCollection](./tablecollection/) | Specifies the table list. |
