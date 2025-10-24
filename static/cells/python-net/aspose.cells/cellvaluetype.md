##CellValueType enumeration
## CellValueType enumeration
Specifies a cell value type.
The CellValueType type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| IS_UNKNOWN | Cell value type is unknown. |
| IS_NULL | Blank cell. Corresponding value should be null. |
| IS_NUMERIC | Cell value is numeric. Corresponding value must be int or double. |
| IS_DATE_TIME | Cell value is datetime. Corresponding value must be DateTime. |
| IS_STRING | Cell value is string. Corresponding value must be string. |
| IS_BOOL | Cell value is boolean. Corresponding value must be bool. |
| IS_ERROR | Cell contains error value. Corresponding value must be error string. |
### See Also
* module [`aspose.cells`](..)
