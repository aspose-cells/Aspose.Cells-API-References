##SetIsExcel2003Compatible Method
'SetIsExcel2003Compatible method. Encapsulates the function that represents setisexcel2003compatible in Go.'
## SetIsExcel2003Compatible function
Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,it will be truncated. if false, a string will not have the aforementioned restriction.The default value is true.
```go
func (instance *PivotTable) SetIsExcel2003Compatible(value bool)  error
```
## Remarks
## See Also
* Class [PivotTable](../)
* Library [Aspose.Cells for Go](../../)
