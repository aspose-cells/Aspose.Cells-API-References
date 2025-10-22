##RevisionInsertSheet Class
'RevisionInsertSheet class. Encapsulates the object that represents revisioninsertsheet in Go.'
## RevisionInsertSheet class
Represents a revision record of a sheet that was inserted.
```go
type RevisionInsertSheet struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionInsertSheet](./newrevisioninsertsheet/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of revision. |
|[GetActionType](./getactiontype/) | Gets the action type of the revision. |
|[GetName](./getname/) | Gets the name of the worksheet. |
|[GetSheetPosition](./getsheetposition/) | Gets the zero based position of the new sheet in the sheet tab bar. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
