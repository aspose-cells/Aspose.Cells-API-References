##QueryTable Class
'QueryTable class. Encapsulates the object that represents querytable in Go.'
## QueryTable class
Represents QueryTable information.
```go
type QueryTable struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetConnectionId](./getconnectionid/) | Gets the connection id of the query table. |
|[GetExternalConnection](./getexternalconnection/) | Gets the relate external connection. |
|[GetName](./getname/) | Gets the name of querytable. |
|[GetResultRange](./getresultrange/) | Gets the range of the result. |
|[GetPreserveFormatting](./getpreserveformatting/) | Returns or sets the PreserveFormatting of the object. |
|[SetPreserveFormatting](./setpreserveformatting/) | Returns or sets the PreserveFormatting of the object. |
|[GetAdjustColumnWidth](./getadjustcolumnwidth/) | Returns or sets the AdjustColumnWidth of the object. |
|[SetAdjustColumnWidth](./setadjustcolumnwidth/) | Returns or sets the AdjustColumnWidth of the object. |
