##Add Method
'Add method. Encapsulates the function that represents add in Go.'
## Add function
Adds a formatting condition and effected cell rang to the FormatConditionsThe FormatConditions can contain up to three conditional formats.References to the other sheets are not allowed in the formulas of conditional formatting.
```go
func (instance *FormatConditionCollection) Add(cellarea *CellArea, type_ FormatConditionType, operatortype OperatorType, formula1 string, formula2 string)  ([]int32,  error)
```
## Remarks
## See Also
* Class [FormatConditionCollection](../)
* Library [Aspose.Cells for Go](../../)
