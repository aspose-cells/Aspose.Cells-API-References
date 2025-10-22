##RevisionMergeConflict Class
'RevisionMergeConflict class. Encapsulates the object that represents revisionmergeconflict in Go.'
## RevisionMergeConflict class
Represents a revision record which indicates that there was a merge conflict.
```go
type RevisionMergeConflict struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionMergeConflict](./newrevisionmergeconflict/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of revision. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
