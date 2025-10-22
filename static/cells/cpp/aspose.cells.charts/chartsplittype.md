##Aspose::Cells::Charts::ChartSplitType enum
'Aspose::Cells::Charts::ChartSplitType enum. Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split in C++.'
## ChartSplitType enum
Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.
```cpp
enum class ChartSplitType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Position | 0 | <br>Represents the data points shall be split between the pie and the second chart by putting the last Split Position of the data points in the second chart. |
| Value | 1 | <br>Represents the data points shall be split between the pie and the second chart by putting the data points with value less than Split Position in the second chart. |
| PercentValue | 2 | <br>Represents the data points shall be split between the pie and the second chart by putting the points with percentage less than Split Position percent in the second chart. |
| Custom | 3 | <br>Represents the data points shall be split between the pie and the second chart according to the Custom Split values. |
| Auto | 4 |  **(Deprecated - Use Series.IsAutoSplit property instead. )** <br>Represents the data points shall be split using the default mechanism for this chart type. |
## See Also
* Namespace [Aspose::Cells::Charts](../)
* Library [Aspose.Cells for C++](../../)
