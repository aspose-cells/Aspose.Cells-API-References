##Series Class
'Series class. Encapsulates the object that represents series in Go.'
## Series class
Encapsulates the object that represents a single data series in a chart.
```go
type Series struct  {
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
|[IsFiltered](./isfiltered/) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
|[SetIsFiltered](./setisfiltered/) | Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart. |
|[GetLayoutProperties](./getlayoutproperties/) | Represents the properties of layout. |
|[Move](./move/) | Moves the series up or down. |
|[GetPoints](./getpoints/) | Gets the collection of points in a series in a chart. |
|[GetArea](./getarea/) | Represents the background area of Series object. |
|[GetBorder](./getborder/) | Represents border of Series object. |
|[GetName](./getname/) | Gets or sets the name of the data series. |
|[SetName](./setname/) | Gets or sets the name of the data series. |
|[GetDisplayName](./getdisplayname/) | Gets the series's name that displays on the chart graph. |
|[GetCountOfDataValues](./getcountofdatavalues/) | Gets the number of the data values. |
|[IsVerticalValues](./isverticalvalues/) | Indicates whether the data source is vertical. |
|[GetValues](./getvalues/) | Represents the Y values of this chart series. |
|[SetValues](./setvalues/) | Represents the Y values of this chart series. |
|[GetValuesFormatCode](./getvaluesformatcode/) | Represents format code of Values's NumberList. |
|[SetValuesFormatCode](./setvaluesformatcode/) | Represents format code of Values's NumberList. |
|[GetXValuesFormatCode](./getxvaluesformatcode/) | Represents format code of X Values's NumberList. |
|[SetXValuesFormatCode](./setxvaluesformatcode/) | Represents format code of X Values's NumberList. |
|[GetXValues](./getxvalues/) | Represents the x values of the chart series. |
|[SetXValues](./setxvalues/) | Represents the x values of the chart series. |
|[GetBubbleSizes](./getbubblesizes/) | Gets or sets the bubble sizes values of the chart series. |
|[SetBubbleSizes](./setbubblesizes/) | Gets or sets the bubble sizes values of the chart series. |
|[GetTrendLines](./gettrendlines/) | Returns all the trendlines of this series. |
|[GetSmooth](./getsmooth/) | Represents curve smoothing.True if curve smoothing is turned on for the line chart or scatter chart.Applies only to line and scatter connected by lines charts. |
|[SetSmooth](./setsmooth/) | Represents curve smoothing.True if curve smoothing is turned on for the line chart or scatter chart.Applies only to line and scatter connected by lines charts. |
|[GetShadow](./getshadow/) | True if the series has a shadow. |
|[SetShadow](./setshadow/) | True if the series has a shadow. |
|[GetHas3DEffect](./gethas3deffect/) | True if the series has a three-dimensional appearance.Applies only to bubble charts. |
|[SetHas3DEffect](./sethas3deffect/) | True if the series has a three-dimensional appearance.Applies only to bubble charts. |
|[GetBar3DShapeType](./getbar3dshapetype/) | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
|[SetBar3DShapeType](./setbar3dshapetype/) | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
|[GetDataLabels](./getdatalabels/) | Represents the DataLabels object for the specified ASeries. |
|[GetType](./gettype/) | Gets or sets a data series' type. |
|[SetType](./settype/) | Gets or sets a data series' type. |
|[GetMarker](./getmarker/) | Gets the Marker</see>. |
|[GetPlotOnSecondAxis](./getplotonsecondaxis/) | Indicates if this series is plotted on second value axis. |
|[SetPlotOnSecondAxis](./setplotonsecondaxis/) | Indicates if this series is plotted on second value axis. |
|[GetXErrorBar](./getxerrorbar/) | Represents X direction error bar of the series. |
|[GetYErrorBar](./getyerrorbar/) | Represents Y direction error bar of the series. |
|[GetHasHiLoLines](./gethashilolines/) | True if the line chart has high-low lines.Applies only to line charts. |
|[SetHasHiLoLines](./sethashilolines/) | True if the line chart has high-low lines.Applies only to line charts. |
|[GetHiLoLines](./gethilolines/) | Returns a HiLoLines object that represents the high-low lines for a series on a line chart.Applies only to line charts. |
|[GetHasSeriesLines](./gethasserieslines/) | True if a stacked column chart or bar chart has series lines orif a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections.Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
|[SetHasSeriesLines](./sethasserieslines/) | True if a stacked column chart or bar chart has series lines orif a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections.Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
|[GetSeriesLines](./getserieslines/) | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart.Applies only to stacked bar and stacked column charts. |
|[GetHasDropLines](./gethasdroplines/) | True if the chart has drop lines.Applies only to line chart or area charts. |
|[SetHasDropLines](./sethasdroplines/) | True if the chart has drop lines.Applies only to line chart or area charts. |
|[GetDropLines](./getdroplines/) | Returns a Line object that represents the drop lines for a series on the line chart or area chart.Applies only to line chart or area charts. |
|[GetHasUpDownBars](./gethasupdownbars/) | True if a line chart has up and down bars.Applies only to line charts. |
|[SetHasUpDownBars](./sethasupdownbars/) | True if a line chart has up and down bars.Applies only to line charts. |
|[GetUpBars](./getupbars/) | Returns an DropBars object that represents the up bars on a line chart.Applies only to line charts. |
|[GetDownBars](./getdownbars/) | Returns a DropBars object that represents the down bars on a line chart.Applies only to line charts. |
|[IsColorVaried](./iscolorvaried/) | Represents if the color of points is varied.The chart must contain only one series. |
|[SetIsColorVaried](./setiscolorvaried/) | Represents if the color of points is varied.The chart must contain only one series. |
|[GetGapWidth](./getgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
|[SetGapWidth](./setgapwidth/) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.The value of this property must be between 0 and 500. |
|[GetFirstSliceAngle](./getfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical).Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
|[SetFirstSliceAngle](./setfirstsliceangle/) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical).Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
|[GetOverlap](./getoverlap/) | Specifies how bars and columns are positioned.Can be a value between – 100 and 100.Applies only to 2-D bar and 2-D column charts. |
|[SetOverlap](./setoverlap/) | Specifies how bars and columns are positioned.Can be a value between – 100 and 100.Applies only to 2-D bar and 2-D column charts. |
|[GetSecondPlotSize](./getsecondplotsize/) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart,as a percentage of the size of the primary pie.Can be a value from 5 to 200. |
|[SetSecondPlotSize](./setsecondplotsize/) | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart,as a percentage of the size of the primary pie.Can be a value from 5 to 200. |
|[GetSplitType](./getsplittype/) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar ofpie chart. |
|[SetSplitType](./setsplittype/) | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar ofpie chart. |
|[GetSplitValue](./getsplitvalue/) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar ona pie of pie or bar of pie chart. |
|[SetSplitValue](./setsplitvalue/) | Returns or sets a value that shall be used to determine which data points are in the second pie or bar ona pie of pie or bar of pie chart. |
|[IsAutoSplit](./isautosplit/) | Indicates whether the threshold value is automatic. |
|[GetBubbleScale](./getbubblescale/) | Gets or sets the scale factor for bubbles in the specified chart group.It can be an integer value from 0 (zero) to 300,corresponding to a percentage of the default size.Applies only to bubble charts. |
|[SetBubbleScale](./setbubblescale/) | Gets or sets the scale factor for bubbles in the specified chart group.It can be an integer value from 0 (zero) to 300,corresponding to a percentage of the default size.Applies only to bubble charts. |
|[GetSizeRepresents](./getsizerepresents/) | Gets or sets what the bubble size represents on a bubble chart. |
|[SetSizeRepresents](./setsizerepresents/) | Gets or sets what the bubble size represents on a bubble chart. |
|[GetShowNegativeBubbles](./getshownegativebubbles/) | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
|[SetShowNegativeBubbles](./setshownegativebubbles/) | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
|[GetDoughnutHoleSize](./getdoughnutholesize/) | Returns or sets the size of the hole in a doughnut chart group.The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
|[SetDoughnutHoleSize](./setdoughnutholesize/) | Returns or sets the size of the hole in a doughnut chart group.The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
|[GetExplosion](./getexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
|[SetExplosion](./setexplosion/) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
|[GetHasRadarAxisLabels](./gethasradaraxislabels/) | True if a radar chart has category axis labels. Applies only to radar charts. |
|[SetHasRadarAxisLabels](./sethasradaraxislabels/) | True if a radar chart has category axis labels. Applies only to radar charts. |
|[GetHasLeaderLines](./gethasleaderlines/) | True if the series has leader lines. |
|[SetHasLeaderLines](./sethasleaderlines/) | True if the series has leader lines. |
|[GetLeaderLines](./getleaderlines/) | Represents leader lines on a chart. Leader lines connect data labels to data points.This object isn’t a collection; there’s no object that represents a single leader line. |
|[GetLegendEntry](./getlegendentry/) | Gets the legend entry according to this series. |
|[GetShapeProperties](./getshapeproperties/) | Gets the ShapePropertyCollection object that holds the visual shape properties of the Series. |
