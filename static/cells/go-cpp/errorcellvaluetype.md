##ErrorCellValueType Enum
'ErrorCellValueType enum. Encapsulates the object that represents errorcellvaluetype in Go.'
## ErrorCellValueType Enum
Represents a cell value which contains an error.
```go
type ErrorCellValueType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Blocked](./blocked/) | Represents the value of a cell containing a #BLOCKED! error. |
|[Busy](./busy/) | Represents the value of a cell containing a #BUSY! error. |
|[Calc](./calc/) | Represents the value of a cell containing a #CALC! error. |
|[Connect](./connect/) | Represents the value of a cell containing a #CONNECT! error. |
|[Name](./name/) | Represents the value of a cell containing a #NAME? error. |
|[Field](./field/) | Represents the value of a cell containing a #FIELD! error. |
|[Spill](./spill/) | Represents the value of a cell containing a #SPILL! error. |
|[Unknown](./unknown/) | Represents the value of a cell containing a #UNKNOWN! error. |
|[TimeOut](./timeout/) | Represents the value of a cell containing a #TIMEOUT! error. |
|[External](./external/) | Represents the value of a cell containing an #EXTERNAL! error. |
