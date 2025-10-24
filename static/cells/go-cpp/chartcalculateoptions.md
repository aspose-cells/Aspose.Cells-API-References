##ChartCalculateOptions Class
'ChartCalculateOptions class. Encapsulates the object that represents chartcalculateoptions in Go.'
## ChartCalculateOptions class
Represents the options for calculating chart.
```go
type ChartCalculateOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewChartCalculateOptions](./newchartcalculateoptions/) | Creates the options for calculating chart. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetUpdateAllPoints](./getupdateallpoints/) | Whether update all data points when performing the chart calculation. Default: False.When you want to get the value for each data point in the chart specifically, set it to true.If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |
|[SetUpdateAllPoints](./setupdateallpoints/) | Whether update all data points when performing the chart calculation. Default: False.When you want to get the value for each data point in the chart specifically, set it to true.If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |
