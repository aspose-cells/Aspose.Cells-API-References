##Class Chart
Aspose.Cells.Charts.Chart class. Encapsulates the object that represents a single Excel chart
## Chart class
Encapsulates the object that represents a single Excel chart.
```csharp
public class Chart
```
## Properties
| Name | Description |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) Gets actual size of chart in unit of pixels. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. The RightAngleAxes property must be True. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | Returns a [`Walls`](./walls/) object that represents the back wall of a 3-D chart. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | Gets the chart's X axis. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | Gets the chart area in the worksheet. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | Represents the chart data table. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | Represents the chartShape; |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | Indicates whether displaying #N/A as blank value. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | Represents the elevation of the 3-D chart view, in degrees. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | Gets a [`SeriesCollection`](../seriescollection/) collection representing the data series that are filtered in the chart. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | Returns a [`Floor`](./floor/) object that represents the walls of a 3-D chart. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width. The value of this property must be between 0 and 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | Indicates whether the chart is a 3d chart. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | Gets the chart legend. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | Gets the line. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | Gets and sets the name of the chart. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | Gets a [`SeriesCollection`](../seriescollection/) collection representing the data series in the chart. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | Represents the page setup description in this chart. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100. This property is ignored if the RightAngleAxes property is True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | Specifies the pivot controls that appear on the chart |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | Represents the way the chart is attached to the cells below it. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | Gets the chart's plot area which includes axis tick labels. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | Gets and sets whether plot by row or column. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | Gets and sets how to plot the empty cells. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) Indicates whether only plot visible cells. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | Indicates whether plot visible cells only. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | Gets and sets the printed chart size. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | Gets the chart's second X axis. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | Gets the chart's second Y axis. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | Gets the chart's series axis. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | Returns all drawing shapes in this chart. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | Gets or sets a value indicating whether the chart displays a data table. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | Returns a [`Walls`](./walls/) object that represents the side wall of a 3-D chart. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | Gets and sets the builtin style. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | Gets the chart's sub-title. Only for ODS format file. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | Gets the chart's title. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | Gets or sets a chart's type. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | Gets the chart's Y axis. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | Returns a [`Walls`](./walls/) object that represents the walls of a 3-D chart. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | Gets the worksheet which contains this chart. |
## Methods
| Name | Description |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | Change chart type with preset template. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | Gets actual size of chart in unit of pixels. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | Gets the data source range of the chart. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | Returns which axes exist on the chart. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | Returns whether the cell refered by the chart. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | Detects if a chart's data source has changed. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) Returns whether the cell refered by the chart. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | Moves the chart to a specified location. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | Refreshes chart's data from pivot table. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | Specifies data range for a chart. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | Switches row/column. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | Gets a 32-bit `Bitmap` object of the chart. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | Gets a 32-bit `Bitmap` object of the chart. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression and ImageOrPrintOptions.Quality attributes are ignored. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) Creates the chart image and saves it to a stream in the specified format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | Creates the chart image and saves it to a stream in the specified format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | Creates the chart image and saves it to a stream in the specified format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | Creates the chart image and saves it to a stream in the Jpeg format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) Creates the chart image and saves it to a file in the specified format. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | Creates the chart image and saves it to a file. The extension of the file name determines the format of the image. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | Creates the chart image and saves it to a file in the specified image type. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) Creates the chart image and saves it to a file in the Jpeg format. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | Creates the chart pdf and saves it to a stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | Saves the chart to a pdf file. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Creates the chart pdf and saves it to a stream. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | Saves the chart to a pdf file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class ChartDemo
{
public static void ChartExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells[0, 1].PutValue("Income");
worksheet.Cells[1, 0].PutValue("Company A");
worksheet.Cells[2, 0].PutValue("Company B");
worksheet.Cells[3, 0].PutValue("Company C");
worksheet.Cells[1, 1].PutValue(10000);
worksheet.Cells[2, 1].PutValue(20000);
worksheet.Cells[3, 1].PutValue(30000);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = worksheet.Charts[chartIndex];
// Set the data range for the chart
chart.SetChartDataRange("A1:B4", true);
// Set chart properties
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";
chart.Style = 2; // Built-in style
// Customize the chart's appearance
chart.ChartObject.Name = "IncomeChart";
chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
chart.PlotVisibleCells = true;
chart.DisplayNaAsBlank = true;
chart.SizeWithWindow = true;
// Customize the chart's axes
chart.CategoryAxis.Title.Text = "Companies";
chart.ValueAxis.Title.Text = "Income";
chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
chart.ValueAxis.MajorTickMark = TickMarkType.Outside;
// Customize the chart's legend
chart.Legend.Position = LegendPositionType.Bottom;
chart.Legend.IsOverLay = false;
// Customize the chart's plot area
chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
chart.PlotArea.Border.IsVisible = false;
// Customize the chart's chart area
chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
chart.ChartArea.Border.IsVisible = false;
// Save the workbook
workbook.Save("ChartExample.xlsx");
workbook.Save("ChartExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
