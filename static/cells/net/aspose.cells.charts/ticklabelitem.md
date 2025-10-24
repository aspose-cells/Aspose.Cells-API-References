##Class TickLabelItem
Aspose.Cells.Charts.TickLabelItem class. Represents a tick label in the chart
## TickLabelItem class
Represents a tick label in the chart.
```csharp
public class TickLabelItem
```
## Properties
| Name | Description |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Height of Ticklabel item in ratio of chart height. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Width of Ticklabel item in ratio of chart width. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | X coordinates of Ticklabel item in ratio of chart width. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Y coordinates of Ticklabel item in ratio of chart height. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartsClassTickLabelItemDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Calculate chart
chart.Calculate();
// Access category axis tick labels
Axis axis = chart.CategoryAxis;
TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;
// Add shapes to mark each tick label position
foreach (TickLabelItem item in tickLabelItems)
{
// Add rectangle around tick label
Shape rectangle = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
item.X,
item.Y,
item.X + item.Width,
item.Y + item.Height);
rectangle.Fill.SolidFill.Transparency = 1;
rectangle.Line.SolidFill.Color = Color.Blue;
// Add circle next to tick label
Shape circle = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Oval,
PlacementType.Move,
item.X + item.Width,
item.Y,
item.X + item.Width + item.Height,
item.Y + item.Height);
circle.Fill.SolidFill.Color = Color.Red;
}
// Save the workbook
workbook.Save("TickLabelItemDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
