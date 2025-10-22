##RevisionFormat Class
'RevisionFormat class. Encapsulates the object that represents revisionformat in Go.'
## RevisionFormat class
Represents a revision record of information about a formatting change.
```go
type RevisionFormat struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionFormat](./newrevisionformat/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of revision. |
|[GetAreas](./getareas/) | The range to which this formatting was applied. |
|[GetStyle](./getstyle/) | Gets the applied style. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
