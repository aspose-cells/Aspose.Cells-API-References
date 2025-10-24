##CellValueType Enum
'CellValueType enum. Encapsulates the object that represents cellvaluetype in Go.'
## CellValueType Enum
Specifies a cell value type.
```go
type CellValueType int32
```
## Fields
| Field | Description |
| --- | --- |
|[IsUnknown](./isunknown/) | Cell value type is unknown. |
|[IsNull](./isnull/) | Blank cell. Corresponding value should be null. |
|[IsNumeric](./isnumeric/) | Cell value is numeric. Corresponding value must be int or double. |
|[IsDateTime](./isdatetime/) | Cell value is datetime. Corresponding value must be DateTime. |
|[IsString](./isstring/) | Cell value is string. Corresponding value must be string. |
|[IsBool](./isbool/) | Cell value is boolean. Corresponding value must be bool. |
|[IsError](./iserror/) | Cell contains error value. Corresponding value must be error string. |
