##RevisionDefinedName Class
'RevisionDefinedName class. Encapsulates the object that represents revisiondefinedname in Go.'
## RevisionDefinedName class
Represents a revision record of a defined name change.
```go
type RevisionDefinedName struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewRevisionDefinedName](./newrevisiondefinedname/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetType](./gettype/) | Represents the type of revision. |
|[GetText](./gettext/) | Gets the text of the defined name. |
|[GetOldFormula](./getoldformula/) | Gets the old formula. |
|[GetNewFormula](./getnewformula/) | Gets the formula. |
|[GetWorksheet](./getworksheet/) | Gets the worksheet. |
|[GetId](./getid/) | Gets the number of this revision. |
