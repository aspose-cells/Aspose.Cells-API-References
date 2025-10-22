##CellWatchCollection Class
'CellWatchCollection class. Encapsulates the object that represents cellwatchcollection in Go.'
## CellWatchCollection class
Represents the collection of cells on this worksheet being watched in the 'watch window'.
```go
type CellWatchCollection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCellWatchCollection](./newcellwatchcollection/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Add_Int_Int](./add_int_int/) | Adds CellWatch with row and column. |
|[Add_String](./add_string/) | Adds CellWatch with the name the of cell. |
|[Get_Int](./get_int/) | Gets and sets CellWatch by index. |
|[Get_String](./get_string/) | Gets and sets CellWatch by the name of the cell. |
|[GetCount](./getcount/) |  |
