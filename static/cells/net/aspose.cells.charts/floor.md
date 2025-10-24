##Class Floor
Aspose.Cells.Charts.Floor class. Encapsulates the object that represents the floor of a 3D chart
## Floor class
Encapsulates the object that represents the floor of a 3-D chart.
```csharp
public class Floor : Area
```
## Properties
| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Gets or sets the background Color of the [`Area`](../../aspose.cells.drawing/area/).(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Gets or sets the border [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Represents a [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) object that contains fill formatting properties for the specified chart or shape.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Gets or sets the foreground Color.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Represents the formatting of the area.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).(Inherited from [`Area`](../../aspose.cells.drawing/area/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class FloorDemo
{
public static void FloorExample()
{
// Instantiate the workbook object
Workbook workbook = new Workbook();
// Get cells collection
Cells cells = workbook.Worksheets[0].Cells;
// Put values in cells
cells["A1"].PutValue(1);
cells["A2"].PutValue(2);
cells["A3"].PutValue(3);
// Get charts collection
ChartCollection charts = workbook.Worksheets[0].Charts;
// Add a new chart
int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);
// Get the newly added chart
Chart chart = charts[index];
// Set chart's nseries
chart.NSeries.Add("A1:A3", true);
// Show data labels
chart.NSeries[0].DataLabels.ShowValue = true;
// Get chart's floor
Floor floor = chart.Floor;
// Set floor's border as red
floor.Border.Color = Color.Red;
// Set fill format
floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);
// Set additional properties
floor.BackgroundColor = Color.LightBlue;
floor.ForegroundColor = Color.DarkBlue;
floor.Formatting = FormattingType.Custom;
floor.InvertIfNegative = true;
floor.Transparency = 0.5;
// Save the file
workbook.Save(@"FloorExample.xlsx");
workbook.Save(@"FloorExample.pdf");
}
}
}
```
### See Also
* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
