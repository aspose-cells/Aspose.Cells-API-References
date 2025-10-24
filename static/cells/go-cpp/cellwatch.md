##CellWatch Class
'CellWatch class. Encapsulates the object that represents cellwatch in Go.'
## CellWatch class
Represents Cell Watch Item in the 'watch window'.
```go
type CellWatch struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCellWatch](./newcellwatch/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetRow](./getrow/) | Gets and sets the row of the cell. |
|[SetRow](./setrow/) | Gets and sets the row of the cell. |
|[GetColumn](./getcolumn/) | Gets and sets the column of the cell. |
|[SetColumn](./setcolumn/) | Gets and sets the column of the cell. |
|[GetCellName](./getcellname/) | Gets and sets the name of the cell. |
|[SetCellName](./setcellname/) | Gets and sets the name of the cell. |
