##SolidFill.Transparency
SolidFill property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## SolidFill.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SolidFillPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.Calculate();
// Add a shape to demonstrate transparency
Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating,
1000, 1000, 2000, 2000);
// Set solid fill with transparency
shape.Fill.SolidFill.Color = Color.Blue;
shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent
// Add another shape for comparison (fully opaque)
Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating,
3000, 1000, 2000, 2000);
shape2.Fill.SolidFill.Color = Color.Blue;
shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)
// Save the workbook
workbook.Save("SolidFillTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
