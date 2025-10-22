##GetSheetsInLoadingOrder Method
'GetSheetsInLoadingOrder method. Encapsulates the function that represents getsheetsinloadingorder in Go.'
## GetSheetsInLoadingOrder function
Specifies the sheets(indices) and order to be loaded.Default is null, that denotes to load all sheets in the default order in template file.If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.
```go
func (instance *LoadFilter) GetSheetsInLoadingOrder()  ([]int32,  error)
```
## Remarks
## See Also
* Class [LoadFilter](../)
* Library [Aspose.Cells for Go](../../)
