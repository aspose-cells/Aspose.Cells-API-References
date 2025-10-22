##ChartSplitType Enum
'ChartSplitType enum. Encapsulates the object that represents chartsplittype in Go.'
## ChartSplitType Enum
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
```go
type ChartSplitType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Position](./position/) | Represents the data points shall be split between the pieand the second chart by putting the last Split Positionof the data points in the second chart |
|[Value](./value/) | Represents the data points shall be split between the pieand the second chart by putting the data points withvalue less than Split Position in the second chart. |
|[PercentValue](./percentvalue/) | Represents the data points shall be split between the pieand the second chart by putting the points withpercentage less than Split Position percent in thesecond chart. |
|[Custom](./custom/) | Represents the data points shall be split between the pieand the second chart according to the Custom Splitvalues. |
|[Auto](./auto/) | Represents the data points shall be split using the defaultmechanism for this chart type. |
