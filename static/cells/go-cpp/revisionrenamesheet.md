##RevisionRenameSheet Class
'RevisionRenameSheet class. Encapsulates the object that represents revisionrenamesheet in Go.'
## RevisionRenameSheet class
Represents a revision of renaming sheet.
```go
type RevisionRenameSheet struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionRenameSheet](./newrevisionrenamesheet/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of the revision. |
|[GetOldName](./getoldname/) | Gets the old name of the worksheet. |
|[GetNewName](./getnewname/) | Gets the new name of the worksheet. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
