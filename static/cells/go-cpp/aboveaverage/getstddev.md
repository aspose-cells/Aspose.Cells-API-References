##GetStdDev Method
'GetStdDev method. Encapsulates the function that represents getstddev in Go.'
## GetStdDev function
Get or set the number of standard deviations to include above or below the average in theconditional formatting rule.The input value must between 0 and 3 (include 0 and 3).Setting this value to 0 means stdDev is not set.The default value is 0.
```go
func (instance *AboveAverage) GetStdDev()  (int32,  error)
```
## Remarks
## See Also
* Class [AboveAverage](../)
* Library [Aspose.Cells for Go](../../)
