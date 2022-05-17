---
title: Chart
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 420
url: /net/aspose.cells.charts/chart/
---
## Chart class

Encapsulates the object that represents a single Excel chart.

```csharp
public class Chart
```

## Properties

| Name | Description |
| --- | --- |
| [ActualChartSize](actualchartsize) { get; } | Gets actual size of chart |
| [AutoScaling](autoscaling) { get; set; } | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [BackWall](backwall) { get; } | Returns a [`Walls`](./walls) object that represents the back wall of a 3-D chart. |
| [CategoryAxis](categoryaxis) { get; } | Gets the chart's X axis. |
| [ChartArea](chartarea) { get; } | Gets the chart area in the worksheet |
| [ChartDataTable](chartdatatable) { get; } | Represents the chart data table. |
| [ChartObject](chartobject) { get; } | Represents the chartShape; |
| [DepthPercent](depthpercent) { get; set; } | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [DisplayNaAsBlank](displaynaasblank) { get; set; } | Indicates whether displaying #N/A as blank value. |
| [Elevation](elevation) { get; set; } | Represents the elevation of the 3-D chart view, in degrees. |
| [FirstSliceAngle](firstsliceangle) { get; set; } | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [Floor](floor) { get; } | Returns a [`Floor`](./floor) object that represents the walls of a 3-D chart. |
| [GapDepth](gapdepth) { get; set; } | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [GapWidth](gapwidth) { get; set; } | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [HeightPercent](heightpercent) { get; set; } | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [HidePivotFieldButtons](hidepivotfieldbuttons) { get; set; } | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart |
| [Is3D](is3d) { get; } | Indicates whether the chart is a 3d chart. |
| [IsRectangularCornered](isrectangularcornered) { get; set; } | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [Legend](legend) { get; } | Gets the chart legend. |
| [Line](line) { get; } | Gets the line. |
| [Name](name) { get; set; } | Gets and sets the name of the chart. |
| [NSeries](nseries) { get; } | Gets a [`SeriesCollection`](../seriescollection) collection representing the data series in the chart. |
| [PageSetup](pagesetup) { get; } | Represents the page setup description in this chart. |
| [Perspective](perspective) { get; set; } | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [PivotOptions](pivotoptions) { get; } | Specifies the pivot controls that appear on the chart |
| [PivotSource](pivotsource) { get; set; } | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [Placement](placement) { get; set; } | Represents the way the chart is attached to the cells below it. |
| [PlotArea](plotarea) { get; } | Gets the chart's plot area which includes axis tick labels. |
| [PlotBy](plotby) { get; } | Gets and sets whether plot by row or column. |
| [PlotEmptyCellsType](plotemptycellstype) { get; set; } | Gets and sets how to plot the empty cells. |
| [PlotVisibleCells](plotvisiblecells) { get; set; } | Indicates whether only plot visible cells. |
| [PrintSize](printsize) { get; set; } | Gets and sets the printed chart size. |
| [RightAngleAxes](rightangleaxes) { get; set; } | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [RotationAngle](rotationangle) { get; set; } | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [SecondCategoryAxis](secondcategoryaxis) { get; } | Gets the chart's second X axis. |
| [SecondValueAxis](secondvalueaxis) { get; } | Gets the chart's second Y axis. |
| [SeriesAxis](seriesaxis) { get; } | Gets the chart's series axis. |
| [Shapes](shapes) { get; } | Returns all drawing shapes in this chart. |
| [ShowDataTable](showdatatable) { get; set; } | Gets or sets a value indicating whether the chart displays a data table. |
| [ShowLegend](showlegend) { get; set; } | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [SideWall](sidewall) { get; } | Returns a [`Walls`](./walls) object that represents the side wall of a 3-D chart. |
| [SizeWithWindow](sizewithwindow) { get; set; } | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [Style](style) { get; set; } | Gets and sets the builtin style. |
| [SubTitle](subtitle) { get; } | Gets the chart's sub-title. Only for ODS format file. |
| [Title](title) { get; } | Gets the chart's title. |
| [Type](type) { get; set; } | Gets or sets a chart's type. |
| [ValueAxis](valueaxis) { get; } | Gets the chart's Y axis. |
| [Walls](walls) { get; } | Returns a [`Walls`](./walls) object that represents the walls of a 3-D chart. |
| [WallsAndGridlines2D](wallsandgridlines2d) { get; set; } | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [Worksheet](worksheet) { get; } | Gets the worksheet which contains this chart. |

## Methods

| Name | Description |
| --- | --- |
| [Calculate](calculate)() | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [GetChartDataRange](getchartdatarange)() | Gets the data source range of the chart . |
| [HasAxis](hasaxis)(AxisType, bool) | Returns which axes exist on the chart. |
| [IsChartDataChanged](ischartdatachanged)() | Detects if a chart's data source has changed. |
| [Move](move)(int, int, int, int) | Moves the chart to a specified location. |
| [RefreshPivotData](refreshpivotdata)() | Refreshes pivot chart's data from it's pivot data source. |
| [SetChartDataRange](setchartdatarange)(string, bool) | Specifies data range for a chart. |
| [SwitchRowColumn](switchrowcolumn)() | Switches row/column. |
| [ToImage](toimage)() | Gets a 32-bit `Bitmap` object of the chart. |
| [ToImage](toimage)(ImageOrPrintOptions) | Gets a 32-bit `Bitmap` object of the chart. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression and ImageOrPrintOptions.Quality attributes are ignored. |
| [ToImage](toimage)(string) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage](toimage)(Stream, ImageFormat) | Creates the chart image and saves it to a stream in the specified format. |
| [ToImage](toimage)(Stream, ImageOrPrintOptions) | Creates the chart image and saves it to a stream in the specified format. |
| [ToImage](toimage)(Stream, long) | Creates the chart image and saves it to a stream in the Jpeg format. |
| [ToImage](toimage)(string, ImageFormat) | Creates the chart image and saves it to a file in the specified format. |
| [ToImage](toimage)(string, ImageOrPrintOptions) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage](toimage)(string, long) | Creates the chart image and saves it to a file in the Jpeg format. |
| [ToPdf](topdf)(Stream) | Creates the chart pdf and saves it to a stream. |
| [ToPdf](topdf)(string) | Saves the chart to a pdf file. |
| [ToPdf](topdf)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Creates the chart pdf and saves it to a stream. |
| [ToPdf](topdf)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Saves the chart to a pdf file. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);

Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex) 
chart.SetChartDataRange("A1:B4", True);
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
