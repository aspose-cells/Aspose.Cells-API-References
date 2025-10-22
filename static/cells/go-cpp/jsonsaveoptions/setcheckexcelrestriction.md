##SetCheckExcelRestriction Method
'SetCheckExcelRestriction method. Encapsulates the function that represents setcheckexcelrestriction in Go.'
## SetCheckExcelRestriction function
Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated.
```go
func (instance *JsonSaveOptions) SetCheckExcelRestriction(value bool)  error
```
## Remarks
## See Also
* Class [JsonSaveOptions](../)
* Library [Aspose.Cells for Go](../../)
