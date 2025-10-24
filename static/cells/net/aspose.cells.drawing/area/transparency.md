##Area.Transparency
Area property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## Area.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AreaPropertyTransparencyDemo
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
// Access the first series
Aspose.Cells.Charts.Series series = chart.NSeries[0];
// Demonstrate Transparency property
Console.WriteLine("Initial area transparency: " + series.Area.Transparency);
Console.WriteLine("Initial border transparency: " + series.Border.Transparency);
// Modify transparency values
series.Area.Transparency = 0.5; // 50% transparent
series.Border.Transparency = 0.2; // 20% transparent
Console.WriteLine("Modified area transparency: " + series.Area.Transparency);
Console.WriteLine("Modified border transparency: " + series.Border.Transparency);
// Save the workbook
workbook.Save("AreaPropertyTransparencyDemo_out.xlsx");
}
}
}
```
### See Also
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
