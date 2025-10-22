##CellValue Class
'CellValue class. Encapsulates the object that represents cellvalue in Go.'
## CellValue class
Represents the cell value and corresponding type.
```go
type CellValue struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCellValue](./newcellvalue/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets/sets the type of cell value. |
|[SetType](./settype/) | Gets/sets the type of cell value. |
|[GetValue](./getvalue/) | Gets/sets the cell value. |
|[SetValue](./setvalue/) | Gets/sets the cell value. |
