##TickLabels.TickLabelItems
TickLabels property. Gets the display tick labels of the axis
## TickLabels.TickLabelItems property
Gets the display tick labels of the axis.
```csharp
public TickLabelItem[] TickLabelItems { get; }
```
### Remarks
Only available after calling [`Calculate`](../../chart/calculate/) method.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyTickLabelItemsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Calculate chart
chart.Calculate();
// Get category axis and its tick labels
Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;
// Add shapes to mark each tick label position
for (int i = 0; i < tickLabelItems.Length; i++)
{
Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
// Add a rectangle around each tick label
Shape shape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
item.X,
item.Y,
item.X + item.Width,
item.Y + item.Height);
shape.Fill.SolidFill.Transparency = 1;
shape.Line.SolidFill.Color = Color.Blue;
}
// Save the workbook
workbook.Save("TickLabelItemsDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
