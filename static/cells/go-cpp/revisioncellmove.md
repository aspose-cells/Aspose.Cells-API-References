##RevisionCellMove Class
'RevisionCellMove class. Encapsulates the object that represents revisioncellmove in Go.'
## RevisionCellMove class
Represents a revision record on a cell(s) that moved.
```go
type RevisionCellMove struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionCellMove](./newrevisioncellmove/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of revision. |
|[GetSourceArea](./getsourcearea/) | Gets the source area. |
|[GetDestinationArea](./getdestinationarea/) | Gets the destination area. |
|[GetSourceWorksheet](./getsourceworksheet/) | Gets the source worksheet. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
