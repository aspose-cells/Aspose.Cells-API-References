##TableStyleCollection Class
'TableStyleCollection class. Encapsulates the object that represents tablestylecollection in Go.'
## TableStyleCollection class
Represents all custom table styles.
```go
type TableStyleCollection struct  {
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
|[GetDefaultTableStyleName](./getdefaulttablestylename/) | Gets and sets the default style name of the table. |
|[SetDefaultTableStyleName](./setdefaulttablestylename/) | Gets and sets the default style name of the table. |
|[GetDefaultPivotStyleName](./getdefaultpivotstylename/) | Gets and sets the  default style name of pivot table . |
|[SetDefaultPivotStyleName](./setdefaultpivotstylename/) | Gets and sets the  default style name of pivot table . |
|[AddTableStyle](./addtablestyle/) | Adds a custom table style. |
|[AddPivotTableStyle](./addpivottablestyle/) | Adds a custom pivot table style. |
|[Get_Int](./get_int/) | Gets the table style by the index. |
|[Get_String](./get_string/) | Gets the table style by the name. |
|[GetBuiltinTableStyle](./getbuiltintablestyle/) | Gets the builtin table style |
|[GetCount](./getcount/) |  |
