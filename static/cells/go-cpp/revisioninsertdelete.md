##RevisionInsertDelete Class
'RevisionInsertDelete class. Encapsulates the object that represents revisioninsertdelete in Go.'
## RevisionInsertDelete class
Represents a revision record of a row/column insert/delete action.
```go
type RevisionInsertDelete struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionInsertDelete](./newrevisioninsertdelete/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of revision. |
|[GetCellArea](./getcellarea/) | Gets the inserting/deleting range. |
|[GetActionType](./getactiontype/) | Gets the action type of this revision. |
|[GetRevisions](./getrevisions/) | Gets revision list by this operation. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
