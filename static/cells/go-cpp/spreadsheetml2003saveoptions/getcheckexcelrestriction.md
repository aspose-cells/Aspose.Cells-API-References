##GetCheckExcelRestriction Method
'GetCheckExcelRestriction method. Encapsulates the function that represents getcheckexcelrestriction in Go.'
## GetCheckExcelRestriction function
Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated.
```go
func (instance *SpreadsheetML2003SaveOptions) GetCheckExcelRestriction()  (bool,  error)
```
## Remarks
## See Also
* Class [SpreadsheetML2003SaveOptions](../)
* Library [Aspose.Cells for Go](../../)
