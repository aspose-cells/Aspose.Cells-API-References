##GetUpdateAllPoints Method
'GetUpdateAllPoints method. Encapsulates the function that represents getupdateallpoints in Go.'
## GetUpdateAllPoints function
Whether update all data points when performing the chart calculation. Default: False.When you want to get the value for each data point in the chart specifically, set it to true.If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
```go
func (instance *ChartCalculateOptions) GetUpdateAllPoints()  (bool,  error)
```
## Remarks
## See Also
* Class [ChartCalculateOptions](../)
* Library [Aspose.Cells for Go](../../)
