##SheetSet Class
'SheetSet class. Encapsulates the object that represents sheetset in Go.'
## SheetSet class
Describes a set of sheets.
```go
type SheetSet struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewSheetSet_int32Array](./newsheetset_int32array/) | Creates a sheet set based on exact sheet indexes. |
|[NewSheetSet_stringArray](./newsheetset_stringarray/) | Creates a sheet set based on exact sheet names. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[SheetSet_GetActive](./sheetset_getactive/) | Gets a set with active sheet of the workbook. |
|[SheetSet_GetVisible](./sheetset_getvisible/) | Gets a set with visible sheets of the workbook in their original order. |
|[SheetSet_GetAll](./sheetset_getall/) | Gets a set with all sheets of the workbook in their original order. |
