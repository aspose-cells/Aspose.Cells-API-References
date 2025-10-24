##RevisionCellComment Class
'RevisionCellComment class. Encapsulates the object that represents revisioncellcomment in Go.'
## RevisionCellComment class
Represents a revision record of a cell comment change.
```go
type RevisionCellComment struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionCellComment](./newrevisioncellcomment/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of revision. |
|[GetRow](./getrow/) | Gets the row index of the which contains a comment. |
|[GetColumn](./getcolumn/) | Gets the column index of the which contains a comment. |
|[GetCellName](./getcellname/) | Gets the name of the cell. |
|[SetCellName](./setcellname/) | Gets the name of the cell. |
|[GetActionType](./getactiontype/) | Gets the action type of the revision. |
|[IsOldComment](./isoldcomment/) | Indicates whether it's an  old comment. |
|[GetOldLength](./getoldlength/) | Gets Length of the comment text added in this revision. |
|[GetNewLength](./getnewlength/) | Gets Length of the comment before this revision was made. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
