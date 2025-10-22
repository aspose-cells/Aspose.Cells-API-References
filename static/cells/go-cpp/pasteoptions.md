##PasteOptions Class
'PasteOptions class. Encapsulates the object that represents pasteoptions in Go.'
## PasteOptions class
Represents the paste special options.
```go
type PasteOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewPasteOptions](./newpasteoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetPasteType](./getpastetype/) | The paste special type. |
|[SetPasteType](./setpastetype/) | The paste special type. |
|[GetSkipBlanks](./getskipblanks/) | Indicates whether skips blank cells. |
|[SetSkipBlanks](./setskipblanks/) | Indicates whether skips blank cells. |
|[GetKeepOldTables](./getkeepoldtables/) | Keeps the tables in the destination range. |
|[SetKeepOldTables](./setkeepoldtables/) | Keeps the tables in the destination range. |
|[GetOnlyVisibleCells](./getonlyvisiblecells/) | True means only copying visible cells. |
|[SetOnlyVisibleCells](./setonlyvisiblecells/) | True means only copying visible cells. |
|[GetTranspose](./gettranspose/) | True to transpose rows and columns when the range is pasted. The default value is False. |
|[SetTranspose](./settranspose/) | True to transpose rows and columns when the range is pasted. The default value is False. |
|[GetOperationType](./getoperationtype/) | Gets and sets the operation type when pasting range. |
|[SetOperationType](./setoperationtype/) | Gets and sets the operation type when pasting range. |
|[GetIgnoreLinksToOriginalFile](./getignorelinkstooriginalfile/) | Ingore links to the original file. |
|[SetIgnoreLinksToOriginalFile](./setignorelinkstooriginalfile/) | Ingore links to the original file. |
