##ExportRangeToJsonOptions Class
'ExportRangeToJsonOptions class. Encapsulates the object that represents exportrangetojsonoptions in Go.'
## ExportRangeToJsonOptions class
Indicates the options that exporting range to json.
```go
type ExportRangeToJsonOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewExportRangeToJsonOptions](./newexportrangetojsonoptions/) | Default constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetHasHeaderRow](./gethasheaderrow/) | Indicates whether the range contains header row. |
|[SetHasHeaderRow](./sethasheaderrow/) | Indicates whether the range contains header row. |
|[GetExportAsString](./getexportasstring/) | Exports the string value of the cells to json. |
|[SetExportAsString](./setexportasstring/) | Exports the string value of the cells to json. |
|[GetExportEmptyCells](./getexportemptycells/) | Indicates whether exporting empty cells as null. |
|[SetExportEmptyCells](./setexportemptycells/) | Indicates whether exporting empty cells as null. |
|[GetIndent](./getindent/) | Indicates the indent. |
|[SetIndent](./setindent/) | Indicates the indent. |
