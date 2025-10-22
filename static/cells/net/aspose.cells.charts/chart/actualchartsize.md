##Chart.ActualChartSize
Chart property. Gets actual size of chart in unit of pixels
## Chart.ActualChartSize property
Gets actual size of chart in unit of pixels.
```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use Chart.GetActualSize() method. This property will be removed 12 months later since July 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartPropertyActualChartSizeDemo
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
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Calculate chart to ensure properties are populated
chart.Calculate();
// Demonstrate ActualChartSize usage
Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");
// Add a shape whose size is based on ActualChartSize
Shape shape = chart.Shapes.AddShapeInChartByScale(
MsoDrawingType.Rectangle,
PlacementType.Move,
0.5,  // x position (relative)
0.5,  // y position (relative)
0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
0.6   // height
);
shape.Fill.SolidFill.Color = Color.Blue;
// Save the workbook
workbook.Save("ChartWithActualSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
