##TickLabelItem.Y
TickLabelItem property. Y coordinates of Ticklabel item in ratio of chart height
## TickLabelItem.Y property
Y coordinates of Ticklabel item in ratio of chart height.
```csharp
public double Y { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class TickLabelItemPropertyYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B1:B3", true);
// Set category axis data using NSERIES instead of CategoryData
chart.NSeries.CategoryData = "A1:A3";
// Calculate chart to ensure tick labels are generated
chart.Calculate();
// Get tick label items from category axis
Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;
// Demonstrate Y property usage by adding shapes aligned with tick labels
for (int i = 0; i < tickLabelItems.Length; i++)
{
Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
// Add a rectangle at each tick label's Y position
Shape shape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
item.X,
item.Y, // Using the Y property of TickLabelItem
item.X + 0.05, // Small width
item.Y + 0.02); // Small height
shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
shape.Line.SolidFill.Color = Color.Black;
}
// Save the workbook
workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
}
}
}
```
### See Also
* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
