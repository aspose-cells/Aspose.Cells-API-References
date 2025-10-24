##TickLabelItem.Width
TickLabelItem property. Width of Ticklabel item in ratio of chart width
## TickLabelItem.Width property
Width of Ticklabel item in ratio of chart width.
```csharp
public double Width { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TickLabelItemPropertyWidthDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
// Access tick label items
Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;
// Demonstrate Width property by adding shapes that match tick label dimensions
for (int i = 0; i < items.Length; i++)
{
Aspose.Cells.Charts.TickLabelItem item = items[i];
// Add rectangle matching tick label dimensions (using Width property)
Shape shape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
item.X,
item.Y,
item.X + item.Width,
item.Y + item.Height);
shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
shape.Line.SolidFill.Color = Color.Black;
}
// Save the workbook
workbook.Save("TickLabelItemWidthDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
