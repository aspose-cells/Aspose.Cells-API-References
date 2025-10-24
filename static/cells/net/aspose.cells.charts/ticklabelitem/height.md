##TickLabelItem.Height
TickLabelItem property. Height of Ticklabel item in ratio of chart height
## TickLabelItem.Height property
Height of Ticklabel item in ratio of chart height.
```csharp
public double Height { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TickLabelItemPropertyHeightDemo
{
public static void Run()
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
// Access category axis tick labels
Axis axis = chart.CategoryAxis;
TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;
// Add shapes to visualize tick label item heights
foreach (TickLabelItem item in tickLabelItems)
{
// Add rectangle showing the tick label item bounds
Shape shape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
item.X,
item.Y,
item.X + item.Width,
item.Y + item.Height);
shape.Fill.SolidFill.Transparency = 1;
shape.Line.SolidFill.Color = Color.Blue;
// Add text showing the height value
Shape textShape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.TextBox,
PlacementType.Move,
item.X,
item.Y - 0.05, // Position above the tick label
0.1,
0.05);
textShape.Text = $"H: {item.Height:F4}";
textShape.Fill.SolidFill.Transparency = 1;
}
// Save the workbook
workbook.Save("TickLabelItemHeightDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
