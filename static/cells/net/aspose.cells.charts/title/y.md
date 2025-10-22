##Title.Y
Title property. Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area
## Title.Y property
Gets or sets the y coordinate of the upper left corner in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Please use Title.YRatioToChart property, instead. Y = YRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TitlePropertyYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set chart title
chart.Title.Text = "Sample Chart";
chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
// Calculate chart to ensure layout is updated
chart.Calculate();
// Add a shape aligned with the title's Y position
Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
2000,
chart.Title.Y, // Using the title's Y property
3000,
chart.Title.Y + 500);
shape.Fill.SolidFill.Color = Color.Blue;
// Save the workbook
workbook.Save("TitlePropertyYDemo_Output.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
