##RevisionCustomView Class
'RevisionCustomView class. Encapsulates the object that represents revisioncustomview in Go.'
## RevisionCustomView class
Represents a revision record of adding or removing a custom view to the workbook
```go
type RevisionCustomView struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionCustomView](./newrevisioncustomview/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Gets the type of revision. |
|[GetActionType](./getactiontype/) | Gets the type of action. |
|[GetGuid](./getguid/) | Gets the globally unique identifier of the custom view. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
