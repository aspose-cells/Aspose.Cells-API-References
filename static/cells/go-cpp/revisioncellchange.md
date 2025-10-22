##RevisionCellChange Class
'RevisionCellChange class. Encapsulates the object that represents revisioncellchange in Go.'
## RevisionCellChange class
Represents the revision that changing cells.
```go
type RevisionCellChange struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionCellChange](./newrevisioncellchange/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of revision. |
|[GetCellName](./getcellname/) | Gets the name of the cell. |
|[GetRow](./getrow/) | Gets the row index of the cell. |
|[GetColumn](./getcolumn/) | Gets the column index of the cell. |
|[IsNewFormatted](./isnewformatted/) | Indicates whether this cell is new formatted. |
|[IsOldFormatted](./isoldformatted/) | Indicates whether this cell is old formatted. |
|[GetOldFormula](./getoldformula/) | Gets the old formula. |
|[GetOldValue](./getoldvalue/) | Gets old value of the cell. |
|[GetNewValue](./getnewvalue/) | Gets new value of the cell. |
|[GetNewFormula](./getnewformula/) | Gets the old formula. |
|[GetNewStyle](./getnewstyle/) | Gets the new style of the cell. |
|[GetOldStyle](./getoldstyle/) | Gets the old style of the cell. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
