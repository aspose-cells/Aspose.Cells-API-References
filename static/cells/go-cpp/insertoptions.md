##InsertOptions Class
'InsertOptions class. Encapsulates the object that represents insertoptions in Go.'
## InsertOptions class
Represents the options of inserting.
```go
type InsertOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewInsertOptions](./newinsertoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCopyFormatType](./getcopyformattype/) |  |
|[SetCopyFormatType](./setcopyformattype/) |  |
|[GetUpdateReference](./getupdatereference/) | Indicates if references in other worksheets will be updated. |
|[SetUpdateReference](./setupdatereference/) | Indicates if references in other worksheets will be updated. |
|[GetFormulaChangeMonitor](./getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the insertion. |
|[SetFormulaChangeMonitor](./setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the insertion. |
