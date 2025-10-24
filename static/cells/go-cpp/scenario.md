##Scenario Class
'Scenario class. Encapsulates the object that represents scenario in Go.'
## Scenario class
Represents an individual scenario.
```go
type Scenario struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetComment](./getcomment/) | Gets and sets the comment of scenario. |
|[SetComment](./setcomment/) | Gets and sets the comment of scenario. |
|[GetName](./getname/) | Gets and sets the name of scenario. |
|[SetName](./setname/) | Gets and sets the name of scenario. |
|[GetUser](./getuser/) | Gets name of user who last changed the scenario. |
|[IsHidden](./ishidden/) | Indicates whether scenario is hidden. |
|[SetIsHidden](./setishidden/) | Indicates whether scenario is hidden. |
|[IsLocked](./islocked/) | Indicates whether scenario is locked for editing when the sheet is protected. |
|[SetIsLocked](./setislocked/) | Indicates whether scenario is locked for editing when the sheet is protected. |
|[GetInputCells](./getinputcells/) | Gets the input cells of scenario. |
