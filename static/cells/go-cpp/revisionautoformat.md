##RevisionAutoFormat Class
'RevisionAutoFormat class. Encapsulates the object that represents revisionautoformat in Go.'
## RevisionAutoFormat class
represents a revision record of information about a formatting change.
```go
type RevisionAutoFormat struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionAutoFormat](./newrevisionautoformat/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of the revision. |
|[GetCellArea](./getcellarea/) | Gets the location where the formatting was applied. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
