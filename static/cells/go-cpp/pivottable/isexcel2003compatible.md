##IsExcel2003Compatible Method
'IsExcel2003Compatible method. Encapsulates the function that represents isexcel2003compatible in Go.'
## IsExcel2003Compatible function
Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable,if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters,it will be truncated. if false, a string will not have the aforementioned restriction.The default value is true.
```go
func (instance *PivotTable) IsExcel2003Compatible()  (bool,  error)
```
## Remarks
## See Also
* Class [PivotTable](../)
* Library [Aspose.Cells for Go](../../)
