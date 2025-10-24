##DeleteOptions Class
'DeleteOptions class. Encapsulates the object that represents deleteoptions in Go.'
## DeleteOptions class
Represents the setting of deleting rows/columns.
```go
type DeleteOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewDeleteOptions](./newdeleteoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetUpdateReference](./getupdatereference/) | Indicates if update references in other worksheets. |
|[SetUpdateReference](./setupdatereference/) | Indicates if update references in other worksheets. |
|[GetFormulaChangeMonitor](./getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
|[SetFormulaChangeMonitor](./setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
