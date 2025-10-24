##DeleteBlankOptions Class
'DeleteBlankOptions class. Encapsulates the object that represents deleteblankoptions in Go.'
## DeleteBlankOptions class
Represents the setting of deleting blank cells/rows/columns.
```go
type DeleteBlankOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewDeleteBlankOptions](./newdeleteblankoptions/) | Default constructor. |
|[NewDeleteBlankOptions_DeleteOptions](./newdeleteblankoptions_deleteoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetEmptyStringAsBlank](./getemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string.Default value is true. |
|[SetEmptyStringAsBlank](./setemptystringasblank/) | Whether one cell will be taken as blank when its value is empty string.Default value is true. |
|[GetEmptyFormulaValueAsBlank](./getemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string.Default value is false. |
|[SetEmptyFormulaValueAsBlank](./setemptyformulavalueasblank/) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string.Default value is false. |
|[GetDrawingsAsBlank](./getdrawingsasblank/) | Whether drawing related objects such as picture, shape, chart... will be taken as blank.Default value is true. |
|[SetDrawingsAsBlank](./setdrawingsasblank/) | Whether drawing related objects such as picture, shape, chart... will be taken as blank.Default value is true. |
|[GetMergedCellsShrinkType](./getmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. |
|[SetMergedCellsShrinkType](./setmergedcellsshrinktype/) | Indicates how to process merged cells when deleting blank rows/columns. |
|[GetStartIndex](./getstartindex/) | Specifies the start row/column index of the range to check and delete blank rows/columns. |
|[SetStartIndex](./setstartindex/) | Specifies the start row/column index of the range to check and delete blank rows/columns. |
|[GetEndIndex](./getendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns.Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
|[SetEndIndex](./setendindex/) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns.Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked. |
|[GetUpdateReference](./getupdatereference/) | Indicates if update references in other worksheets. |
|[SetUpdateReference](./setupdatereference/) | Indicates if update references in other worksheets. |
|[GetFormulaChangeMonitor](./getformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
|[SetFormulaChangeMonitor](./setformulachangemonitor/) | Gets/sets the monitor for tracking changes caused by the deletion. |
