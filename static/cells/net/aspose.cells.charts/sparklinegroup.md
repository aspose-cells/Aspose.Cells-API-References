##Class SparklineGroup
Aspose.Cells.Charts.SparklineGroup class. Sparkline is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type display settings and axis settings for the sparklines
## SparklineGroup class
[`Sparkline`](../sparkline/) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.
```csharp
public class SparklineGroup
```
## Properties
| Name | Description |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden/) { get; set; } | Indicates whether to show data in hidden rows and columns. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor/) { get; set; } | Gets and sets the color of the first point of data in the sparkline group. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor/) { get; set; } | Gets and sets the color of the highest points of data in the sparkline group. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor/) { get; set; } | Gets and sets the color of the horizontal axis in the sparkline group. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/) { get; set; } | Represents the range that contains the date values for the sparkline data. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor/) { get; set; } | Gets and sets the color of the last point of data in the sparkline group. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight/) { get; set; } | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor/) { get; set; } | Gets and sets the color of the lowest points of data in the sparkline group. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor/) { get; set; } | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor/) { get; set; } | Gets and sets the color of the negative values on the sparkline group. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype/) { get; set; } | Indicates how to plot empty cells. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft/) { get; set; } | Indicates whether the plot data is right to left. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle/) { get; set; } | Gets and sets the preset style type of the sparkline group. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor/) { get; set; } | Gets and sets the color of the sparklines in the sparkline group. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint/) { get; set; } | Indicates whether to highlight the first point of data in the sparkline group. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint/) { get; set; } | Indicates whether to highlight the highest points of data in the sparkline group. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis/) { get; set; } | Indicates whether to show the sparkline horizontal axis. The horizontal axis appears if the sparkline has data that crosses the zero axis. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint/) { get; set; } | Indicates whether to highlight the last point of data in the sparkline group. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint/) { get; set; } | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers/) { get; set; } | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints/) { get; set; } | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection/) { get; } | (**Obsolete.**) Gets the collection of [`Sparkline`](../sparkline/) object. |
| [Sparklines](../../aspose.cells.charts/sparklinegroup/sparklines/) { get; } | Gets the collection of [`Sparkline`](../sparkline/) object. |
| [Type](../../aspose.cells.charts/sparklinegroup/type/) { get; set; } | Indicates the sparkline type of the sparkline group. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/) { get; set; } | Gets and sets the custom maximum value for the vertical axis. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/) { get; set; } | Represents the vertical axis maximum value type. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue/) { get; set; } | Gets and sets the custom minimum value for the vertical axis. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/) { get; set; } | Represents the vertical axis minimum value type. |
## Methods
| Name | Description |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges/)(string, bool, CellArea) | Resets the data range and location range of the sparkline group. This method will clear original sparkline items in the group and creates new sparkline items for the new ranges. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class SparklineGroupDemo
{
public static void SparklineGroupExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the worksheet
sheet.Cells["A1"].PutValue(5);
sheet.Cells["B1"].PutValue(2);
sheet.Cells["C1"].PutValue(1);
sheet.Cells["D1"].PutValue(3);
// Define the CellArea for the sparkline
CellArea ca = new CellArea
{
StartColumn = 4,
EndColumn = 4,
StartRow = 0,
EndRow = 0
};
// Add a sparkline group to the worksheet
int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
SparklineGroup group = sheet.SparklineGroups[idx];
// Add sparklines to the group
group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
// Create CellsColor for series color
CellsColor seriesColor = workbook.CreateCellsColor();
seriesColor.Color = Color.Orange;
group.SeriesColor = seriesColor;
// Set the high points are colored green and the low points are colored red
group.ShowHighPoint = true;
group.ShowLowPoint = true;
CellsColor highPointColor = workbook.CreateCellsColor();
highPointColor.Color = Color.Green;
group.HighPointColor = highPointColor;
CellsColor lowPointColor = workbook.CreateCellsColor();
lowPointColor.Color = Color.Red;
group.LowPointColor = lowPointColor;
// Set line weight
group.LineWeight = 1.0;
// Set additional properties
group.PresetStyle = SparklinePresetStyleType.Style1;
group.Type = SparklineType.Line;
group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
group.DisplayHidden = true;
group.ShowNegativePoints = true;
CellsColor negativePointsColor = workbook.CreateCellsColor();
negativePointsColor.Color = Color.Blue;
group.NegativePointsColor = negativePointsColor;
group.ShowFirstPoint = true;
CellsColor firstPointColor = workbook.CreateCellsColor();
firstPointColor.Color = Color.Purple;
group.FirstPointColor = firstPointColor;
group.ShowLastPoint = true;
CellsColor lastPointColor = workbook.CreateCellsColor();
lastPointColor.Color = Color.Yellow;
group.LastPointColor = lastPointColor;
group.ShowMarkers = true;
CellsColor markersColor = workbook.CreateCellsColor();
markersColor.Color = Color.Black;
group.MarkersColor = markersColor;
group.PlotRightToLeft = false;
CellsColor horizontalAxisColor = workbook.CreateCellsColor();
horizontalAxisColor.Color = Color.Gray;
group.HorizontalAxisColor = horizontalAxisColor;
group.ShowHorizontalAxis = true;
group.HorizontalAxisDateRange = "A1:D1";
group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
group.VerticalAxisMaxValue = 10.0;
group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Group;
group.VerticalAxisMinValue = 0.0;
// Save the workbook
workbook.Save("SparklineGroupExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
