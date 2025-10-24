##SetReferToSheetWithSameName Method
'SetReferToSheetWithSameName method. Encapsulates the function that represents setrefertosheetwithsamename in Go.'
## SetReferToSheetWithSameName function
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one,the copied formulas should refer to source workbook.However, for some situations user may need the copied formulas refer to worksheets with the same namein the same workbook, such as when those worksheets have been copied before this copy operation,then this property should be kept as true.
```go
func (instance *CopyOptions) SetReferToSheetWithSameName(value bool)  error
```
## Remarks
## See Also
* Class [CopyOptions](../)
* Library [Aspose.Cells for Go](../../)
