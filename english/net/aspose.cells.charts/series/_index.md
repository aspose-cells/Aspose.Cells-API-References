---
title: Series
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 810
url: /net/aspose.cells.charts/series/
---
## Series class

Encapsulates the object that represents a single data series in a chart.

```csharp
public class Series
```

## Properties

| Name | Description |
| --- | --- |
| [Area](area) { get; } | Represents the background area of Series object. |
| [Bar3DShapeType](bar3dshapetype) { get; set; } | Gets or sets the 3D shape type used with the 3-D bar or column chart. |
| [Border](border) { get; } | Represents border of Series object. |
| [BubbleScale](bubblescale) { get; set; } | Gets or sets the scale factor for bubbles in the specified chart group. It can be an integer value from 0 (zero) to 300, corresponding to a percentage of the default size. Applies only to bubble charts. |
| [BubbleSizes](bubblesizes) { get; set; } | Gets or sets the bubble sizes values of the chart series. |
| [CountOfDataValues](countofdatavalues) { get; } | Gets the number of the data values. |
| [DataLabels](datalabels) { get; } | Represents the DataLabels object for the specified ASeries. |
| [DisplayName](displayname) { get; } | Gets the series's name that displays on the chart graph. |
| [DoughnutHoleSize](doughnutholesize) { get; set; } | Returns or sets the size of the hole in a doughnut chart group. The hole size is expressed as a percentage of the chart size, between 10 and 90 percent. |
| [DownBars](downbars) { get; } | Returns a [`DropBars`](../dropbars) object that represents the down bars on a line chart. Applies only to line charts. |
| [DropLines](droplines) { get; } | Returns a [`Line`](../../aspose.cells.drawing/line) object that represents the drop lines for a series on the line chart or area chart. Applies only to line chart or area charts. |
| [Explosion](explosion) { get; set; } | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [FirstSliceAngle](firstsliceangle) { get; set; } | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [GapWidth](gapwidth) { get; set; } | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [Has3DEffect](has3deffect) { get; set; } | True if the series has a three-dimensional appearance. Applies only to bubble charts. |
| [HasDropLines](hasdroplines) { get; set; } | True if the chart has drop lines. Applies only to line chart or area charts. |
| [HasHiLoLines](hashilolines) { get; set; } | True if the line chart has high-low lines. Applies only to line charts. |
| [HasLeaderLines](hasleaderlines) { get; set; } | True if the series has leader lines. |
| [HasRadarAxisLabels](hasradaraxislabels) { get; set; } | True if a radar chart has category axis labels. Applies only to radar charts. |
| [HasSeriesLines](hasserieslines) { get; set; } | True if a stacked column chart or bar chart has series lines or if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts. |
| [HasUpDownBars](hasupdownbars) { get; set; } | True if a line chart has up and down bars. Applies only to line charts. |
| [HiLoLines](hilolines) { get; } | Returns a HiLoLines object that represents the high-low lines for a series on a line chart. Applies only to line charts. |
| [IsAutoSplit](isautosplit) { get; } | Indicates whether the threshold value is automatic. |
| [IsColorVaried](iscolorvaried) { get; set; } | Represents if the color of points is varied. The chart must contain only one series. |
| [IsVerticalValues](isverticalvalues) { get; } | Indicates whether the data source is vertical. |
| [LayoutProperties](layoutproperties) { get; } | Represents the properties of layout. |
| [LeaderLines](leaderlines) { get; } | Represents leader lines on a chart. Leader lines connect data labels to data points. This object isn’t a collection; there’s no object that represents a single leader line. |
| [LegendEntry](legendentry) { get; } | Gets the legend entry according to this series. |
| [Marker](marker) { get; } | Gets the [`marker`](./marker). |
| [Name](name) { get; set; } | Gets or sets the name of the data series. |
| [Overlap](overlap) { get; set; } | Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts. |
| [PlotOnSecondAxis](plotonsecondaxis) { get; set; } | Indicates if this series is plotted on second value axis. |
| [Points](points) { get; } | Gets the collection of points in a series in a chart. |
| [SecondPlotSize](secondplotsize) { get; set; } | Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, as a percentage of the size of the primary pie. Can be a value from 5 to 200. |
| [SeriesLines](serieslines) { get; } | Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts. |
| [Shadow](shadow) { get; set; } | True if the series has a shadow. |
| [ShapeProperties](shapeproperties) { get; } | Gets the  object that holds the visual shape properties of the Series. |
| [ShowNegativeBubbles](shownegativebubbles) { get; set; } | True if negative bubbles are shown for the chart group. Valid only for bubble charts. |
| [SizeRepresents](sizerepresents) { get; set; } | Gets or sets what the bubble size represents on a bubble chart. |
| [Smooth](smooth) { get; set; } | Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts. |
| [SplitType](splittype) { get; set; } | Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [SplitValue](splitvalue) { get; set; } | Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart. |
| [TrendLines](trendlines) { get; } | Returns an object that represents a collection of all the trendlines for the series. |
| [Type](type) { get; set; } | Gets or sets a data series' type. |
| [UpBars](upbars) { get; } | Returns an DropBars object that represents the up bars on a line chart. Applies only to line charts. |
| [Values](values) { get; set; } | Represents the data of the chart series. |
| [ValuesFormatCode](valuesformatcode) { get; set; } | Represents format code of Values‘s NumberList. |
| [XErrorBar](xerrorbar) { get; } | Represents X direction error bar of the series. |
| [XValues](xvalues) { get; set; } | Represents the x values of the chart series. |
| [YErrorBar](yerrorbar) { get; } | Represents Y direction error bar of the series. |

## Methods

| Name | Description |
| --- | --- |
| [Move](move)(int) | Moves the series up or down. |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Adding a sample value to "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Adding a sample value to "A2" cell
worksheet.Cells["A2"].PutValue(100);
//Adding a sample value to "A3" cell
worksheet.Cells["A3"].PutValue(150);
//Adding a sample value to "A4" cell
worksheet.Cells["A4"].PutValue(200);
//Adding a sample value to "B1" cell
worksheet.Cells["B1"].PutValue(60);
//Adding a sample value to "B2" cell
worksheet.Cells["B2"].PutValue(32);
//Adding a sample value to "B3" cell
worksheet.Cells["B3"].PutValue(50);
//Adding a sample value to "B4" cell
worksheet.Cells["B4"].PutValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.Cells["C1"].PutValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.Cells["C2"].PutValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.Cells["C3"].PutValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.Cells["C4"].PutValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
int seriesIndex = chart.NSeries.Add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4";
Series series = chart.NSeries[seriesIndex];
//Setting the values of the series.
series.Values = "=B1:B4";
//Changing the chart type of the series.
series.Type = ChartType.Line;
//Setting marker properties.
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.ForegroundColorSetType = FormattingType.Automatic;
series.Marker.ForegroundColor = System.Drawing.Color.Black;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;

//do your business

//Saving the Excel file
workbook.Save("C:\\book1.xls");

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Adding a new worksheet to the Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Obtaining the reference of the newly added worksheet by passing its sheet index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Adding a chart to the worksheet
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accessing the instance of the newly added chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Setting the data source for the category data of NSeries
chart.NSeries.CategoryData = "C1:C4"
Dim series As Series = chart.NSeries(seriesIndex)
'Setting the values of the series.
series.Values = "=B1:B4"
'Changing the chart type of the series.
series.Type = ChartType.Line
'Setting marker properties.
series.Marker.MarkerStyle = ChartMarkerType.Circle
series.Marker.ForegroundColorSetType = FormattingType.Automatic
series.Marker.ForegroundColor = System.Drawing.Color.Black
series.Marker.BackgroundColorSetType = FormattingType.Automatic
'Saving the Excel file
workbook.Save("C:\\book1.xls")
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
