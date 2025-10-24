##Class Walls
Aspose.Cells.Charts.Walls class. Encapsulates the object that represents the walls of a 3D chart
## Walls class
Encapsulates the object that represents the walls of a 3-D chart.
```csharp
public class Walls : Floor
```
## Properties
| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Gets or sets the background Color of the [`Area`](../../aspose.cells.drawing/area/).(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Gets or sets the border [`Line`](../../aspose.cells.drawing/line/).(Inherited from [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Represents a [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) object that contains fill formatting properties for the specified chart or shape.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Gets or sets the foreground Color.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Represents the formatting of the area.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
## Methods
| Name | Description |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Gets the number of cube points after calls Chart.Calculate() method. |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class WallsDemo
{
public static void WallsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a 3D chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate the chart to update its properties
chart.Calculate();
// Access the walls of the 3D chart
Walls walls = chart.Walls;
// Set properties of the walls
walls.BackgroundColor = Color.LightBlue;
walls.ForegroundColor = Color.DarkBlue;
walls.Formatting = FormattingType.Custom;
walls.InvertIfNegative = true;
walls.Transparency = 0.5;
// Access the border of the walls and set its properties
Line border = walls.Border;
border.Color = Color.Red;
border.Style = LineType.Solid;
// Print some properties of the walls
Console.WriteLine("CenterX: " + walls.CenterX);
Console.WriteLine("CenterY: " + walls.CenterY);
Console.WriteLine("Width: " + walls.Width);
Console.WriteLine("Depth: " + walls.Depth);
Console.WriteLine("Height: " + walls.Height);
Console.WriteLine("CenterXPx: " + walls.CenterXPx);
Console.WriteLine("CenterYPx: " + walls.CenterYPx);
Console.WriteLine("WidthPx: " + walls.WidthPx);
Console.WriteLine("DepthPx: " + walls.DepthPx);
Console.WriteLine("HeightPx: " + walls.HeightPx);
// Save the workbook
workbook.Save("WallsExample.xlsx");
}
}
}
```
### See Also
* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
