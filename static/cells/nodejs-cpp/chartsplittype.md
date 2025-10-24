##ChartSplitType
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
## ChartSplitType enumeration
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Position | `0` | Represents the data points shall be split between the pie and the second chart by putting the last Split Position of the data points in the second chart |
| Value | `1` | Represents the data points shall be split between the pie and the second chart by putting the data points with value less than Split Position in the second chart. |
| PercentValue | `2` | Represents the data points shall be split between the pie and the second chart by putting the points with percentage less than Split Position percent in the second chart. |
| Custom | `3` | Represents the data points shall be split between the pie and the second chart according to the Custom Split values. |
| Auto | `4` | Represents the data points shall be split using the default mechanism for this chart type. |
