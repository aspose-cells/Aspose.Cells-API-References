##CellValueType
Specifies a cell value type.
## CellValueType enumeration
Specifies a cell value type.
### Values
| Name | Value | Description |
| --- | --- | --- |
| IsUnknown | `0` | Cell value type is unknown. |
| IsNull | `1` | Blank cell. Corresponding value should be null. |
| IsNumeric | `2` | Cell value is numeric. Corresponding value must be int or double. |
| IsDateTime | `4` | Cell value is datetime. Corresponding value must be DateTime. |
| IsString | `8` | Cell value is string. Corresponding value must be string. |
| IsBool | `16` | Cell value is boolean. Corresponding value must be bool. |
| IsError | `32` | Cell contains error value. Corresponding value must be error string. |
