##CopyOptions Class
'CopyOptions class. Encapsulates the object that represents copyoptions in Go.'
## CopyOptions class
Represents the copy options.
```go
type CopyOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewCopyOptions](./newcopyoptions/) | CopyOptions constructor. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetKeepMacros](./getkeepmacros/) | Indicates whether keeping macros; |
|[SetKeepMacros](./setkeepmacros/) | Indicates whether keeping macros; |
|[GetExtendToAdjacentRange](./getextendtoadjacentrange/) | Indicates whether extend ranges when copying the range to adjacent range. |
|[SetExtendToAdjacentRange](./setextendtoadjacentrange/) | Indicates whether extend ranges when copying the range to adjacent range. |
|[GetCopyNames](./getcopynames/) | Indicates whether copying the names. |
|[SetCopyNames](./setcopynames/) | Indicates whether copying the names. |
|[GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | If the formula is not valid for the dest destination, only copy values. |
|[SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | If the formula is not valid for the dest destination, only copy values. |
|[GetColumnCharacterWidth](./getcolumncharacterwidth/) | Indicates whether copying column width in unit of characters. |
|[SetColumnCharacterWidth](./setcolumncharacterwidth/) | Indicates whether copying column width in unit of characters. |
|[GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one,the copied formulas should refer to source workbook.However, for some situations user may need the copied formulas refer to worksheets with the same namein the same workbook, such as when those worksheets have been copied before this copy operation,then this property should be kept as true. |
|[SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one,the copied formulas should refer to source workbook.However, for some situations user may need the copied formulas refer to worksheets with the same namein the same workbook, such as when those worksheets have been copied before this copy operation,then this property should be kept as true. |
|[GetReferToDestinationSheet](./getrefertodestinationsheet/) | When copying the range in the same file and the chart refers to the source sheet,False means the copied chart's data source will not be changed.True means the copied chart's data source refers to the destination sheet. |
|[SetReferToDestinationSheet](./setrefertodestinationsheet/) | When copying the range in the same file and the chart refers to the source sheet,False means the copied chart's data source will not be changed.True means the copied chart's data source refers to the destination sheet. |
