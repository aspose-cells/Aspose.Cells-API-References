##ChartPoint.BorderWidthPx
ChartPoint property. Gets the width of border in units of pixels after calls Chart.Calculate method
## ChartPoint.BorderWidthPx property
Gets the width of border in units of pixels after calls Chart.Calculate() method.
```csharp
public int BorderWidthPx { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class ChartPointPropertyBorderWidthPxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["A5"].PutValue("Q4");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1200);
worksheet.Cells["B3"].PutValue(1500);
worksheet.Cells["B4"].PutValue(1800);
worksheet.Cells["B5"].PutValue(2100);
// Add a chart and set its data range
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Calculate the chart to ensure properties are populated
chart.Calculate();
// Get the first chart point in the first series
ChartPoint point = chart.NSeries[0].Points[0];
// Display the current border width
Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);
// Note: BorderWidthPx is read-only, so we can't set it directly
// Instead, we can modify the border through the Border property
if (point.Border != null)
{
// Change the border width by setting the weight using WeightType enum
point.Border.Weight = WeightType.MediumLine; // Medium weight border
}
// Recalculate to update the BorderWidthPx value
chart.Calculate();
// Display the new border width in pixels
Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);
// Save the workbook
workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
