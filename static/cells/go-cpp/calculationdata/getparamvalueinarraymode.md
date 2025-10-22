##GetParamValueInArrayMode Method
'GetParamValueInArrayMode method. Encapsulates the function that represents getparamvalueinarraymode in Go.'
## GetParamValueInArrayMode function
Gets the value(s) of the parameter at given index.If the parameter is some kind of expression that needs to be calculated,then it will be calculated in array mode.
```go
func (instance *CalculationData) GetParamValueInArrayMode(index int32, maxrowcount int32, maxcolumncount int32)  ([][]Object,  error)
```
## Remarks
## See Also
* Class [CalculationData](../)
* Library [Aspose.Cells for Go](../../)
