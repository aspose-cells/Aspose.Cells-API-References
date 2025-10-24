##RevisionQueryTable Class
'RevisionQueryTable class. Encapsulates the object that represents revisionquerytable in Go.'
## RevisionQueryTable class
Represents a revision of a query table field change.
```go
type RevisionQueryTable struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionQueryTable](./newrevisionquerytable/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of the revision. |
|[GetCellArea](./getcellarea/) | Gets the location of the affected query table. |
|[GetFieldId](./getfieldid/) | Gets ID of the specific query table field that was removed. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
