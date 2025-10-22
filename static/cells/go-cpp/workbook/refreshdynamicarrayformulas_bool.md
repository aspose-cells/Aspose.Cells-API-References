##RefreshDynamicArrayFormulas_Bool Method
'RefreshDynamicArrayFormulas_Bool method. Encapsulates the function that represents refreshdynamicarrayformulas in Go.'
## RefreshDynamicArrayFormulas_Bool function
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.
```go
func (instance *Workbook) RefreshDynamicArrayFormulas_Bool(calculate bool)  error
```
## Remarks
## See Also
* Class [Workbook](../)
* Library [Aspose.Cells for Go](../../)
