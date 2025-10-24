##ChartPoint.YValue
ChartPoint property. Gets or sets the Y value of the chart point
## ChartPoint.YValue property
Gets or sets the Y value of the chart point.
```csharp
public object YValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPointPropertyYValueDemo
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
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Get the first series points
Series series = chart.NSeries[0];
var points = series.Points;
// Demonstrate YValue property
Console.WriteLine("Y Values of Chart Points:");
for (int i = 0; i < points.Count; i++)
{
Console.WriteLine($"Point {i + 1}: {points[i].YValue}");
}
// Modify a point's YValue
points[2].YValue = 50;
Console.WriteLine($"\nModified Point 3 YValue to: {points[2].YValue}");
// Save the workbook
workbook.Save("ChartPointYValueDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
