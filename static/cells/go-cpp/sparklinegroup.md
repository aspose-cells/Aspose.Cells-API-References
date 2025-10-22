##SparklineGroup Class
'SparklineGroup class. Encapsulates the object that represents sparklinegroup in Go.'
## SparklineGroup class
```go
type SparklineGroup struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[ResetRanges](./resetranges/) | Resets the data range and location range of the sparkline group.This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |
|[GetPresetStyle](./getpresetstyle/) | Gets and sets the preset style type of the sparkline group. |
|[SetPresetStyle](./setpresetstyle/) | Gets and sets the preset style type of the sparkline group. |
|[GetSparklines](./getsparklines/) | Gets the collection of Sparkline object. |
|[GetType](./gettype/) | Indicates the sparkline type of the sparkline group. |
|[SetType](./settype/) | Indicates the sparkline type of the sparkline group. |
|[GetPlotEmptyCellsType](./getplotemptycellstype/) | Indicates how to plot empty cells. |
|[SetPlotEmptyCellsType](./setplotemptycellstype/) | Indicates how to plot empty cells. |
|[GetDisplayHidden](./getdisplayhidden/) | Indicates whether to show data in hidden rows and columns. |
|[SetDisplayHidden](./setdisplayhidden/) | Indicates whether to show data in hidden rows and columns. |
|[GetShowHighPoint](./getshowhighpoint/) | Indicates whether to highlight the highest points of data in the sparkline group. |
|[SetShowHighPoint](./setshowhighpoint/) | Indicates whether to highlight the highest points of data in the sparkline group. |
|[GetHighPointColor](./gethighpointcolor/) | Gets and sets the color of the highest points of data in the sparkline group. |
|[SetHighPointColor](./sethighpointcolor/) | Gets and sets the color of the highest points of data in the sparkline group. |
|[GetShowLowPoint](./getshowlowpoint/) | Indicates whether to highlight the lowest points of data in the sparkline group. |
|[SetShowLowPoint](./setshowlowpoint/) | Indicates whether to highlight the lowest points of data in the sparkline group. |
|[GetLowPointColor](./getlowpointcolor/) | Gets and sets the color of the lowest points of data in the sparkline group. |
|[SetLowPointColor](./setlowpointcolor/) | Gets and sets the color of the lowest points of data in the sparkline group. |
|[GetShowNegativePoints](./getshownegativepoints/) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
|[SetShowNegativePoints](./setshownegativepoints/) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
|[GetNegativePointsColor](./getnegativepointscolor/) | Gets and sets the color of the negative values on the sparkline group. |
|[SetNegativePointsColor](./setnegativepointscolor/) | Gets and sets the color of the negative values on the sparkline group. |
|[GetShowFirstPoint](./getshowfirstpoint/) | Indicates whether to highlight the first point of data in the sparkline group. |
|[SetShowFirstPoint](./setshowfirstpoint/) | Indicates whether to highlight the first point of data in the sparkline group. |
|[GetFirstPointColor](./getfirstpointcolor/) | Gets and sets the color of the first point of data in the sparkline group. |
|[SetFirstPointColor](./setfirstpointcolor/) | Gets and sets the color of the first point of data in the sparkline group. |
|[GetShowLastPoint](./getshowlastpoint/) | Indicates whether to highlight the last point of data in the sparkline group. |
|[SetShowLastPoint](./setshowlastpoint/) | Indicates whether to highlight the last point of data in the sparkline group. |
|[GetLastPointColor](./getlastpointcolor/) | Gets and sets the color of the last point of data in the sparkline group. |
|[SetLastPointColor](./setlastpointcolor/) | Gets and sets the color of the last point of data in the sparkline group. |
|[GetShowMarkers](./getshowmarkers/) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
|[SetShowMarkers](./setshowmarkers/) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
|[GetMarkersColor](./getmarkerscolor/) | Gets and sets the color of points in each line sparkline in the sparkline group. |
|[SetMarkersColor](./setmarkerscolor/) | Gets and sets the color of points in each line sparkline in the sparkline group. |
|[GetSeriesColor](./getseriescolor/) | Gets and sets the color of the sparklines in the sparkline group. |
|[SetSeriesColor](./setseriescolor/) | Gets and sets the color of the sparklines in the sparkline group. |
|[GetPlotRightToLeft](./getplotrighttoleft/) | Indicates whether the plot data is right to left. |
|[SetPlotRightToLeft](./setplotrighttoleft/) | Indicates whether the plot data is right to left. |
|[GetLineWeight](./getlineweight/) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
|[SetLineWeight](./setlineweight/) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
|[GetHorizontalAxisColor](./gethorizontalaxiscolor/) | Gets and sets the color of the horizontal axis in the sparkline group. |
|[SetHorizontalAxisColor](./sethorizontalaxiscolor/) | Gets and sets the color of the horizontal axis in the sparkline group. |
|[GetShowHorizontalAxis](./getshowhorizontalaxis/) | Indicates whether to show the sparkline horizontal axis.The horizontal axis appears if the sparkline has data that crosses the zero axis. |
|[SetShowHorizontalAxis](./setshowhorizontalaxis/) | Indicates whether to show the sparkline horizontal axis.The horizontal axis appears if the sparkline has data that crosses the zero axis. |
|[GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | Represents the range that contains the date values for the sparkline data. |
|[SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | Represents the range that contains the date values for the sparkline data. |
|[GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | Represents the vertical axis maximum value type. |
|[SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | Represents the vertical axis maximum value type. |
|[GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | Gets and sets the custom maximum value for the vertical axis. |
|[SetVerticalAxisMaxValue](./setverticalaxismaxvalue/) | Gets and sets the custom maximum value for the vertical axis. |
|[GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | Represents the vertical axis minimum value type. |
|[SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | Represents the vertical axis minimum value type. |
|[GetVerticalAxisMinValue](./getverticalaxisminvalue/) | Gets and sets the custom minimum value for the vertical axis. |
|[SetVerticalAxisMinValue](./setverticalaxisminvalue/) | Gets and sets the custom minimum value for the vertical axis. |
