##Axis.IsAutomaticMaxValue
Axis property. Indicates whether the max value is automatically assigned
## Axis.IsAutomaticMaxValue property
Indicates whether the max value is automatically assigned.
```csharp
public bool IsAutomaticMaxValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsAutomaticMaxValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the value axis
Axis valueAxis = chart.ValueAxis;
// Demonstrate IsAutomaticMaxValue property
Console.WriteLine("Initial IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
Console.WriteLine("Initial MaxValue: " + valueAxis.MaxValue);
// Disable automatic max value and set custom value
valueAxis.IsAutomaticMaxValue = false;
valueAxis.MaxValue = 40;
Console.WriteLine("After change - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
Console.WriteLine("After change - MaxValue: " + valueAxis.MaxValue);
// Re-enable automatic max value
valueAxis.IsAutomaticMaxValue = true;
Console.WriteLine("After re-enabling - IsAutomaticMaxValue: " + valueAxis.IsAutomaticMaxValue);
Console.WriteLine("After re-enabling - MaxValue: " + valueAxis.MaxValue);
// Save the workbook
workbook.Save("AxisPropertyIsAutomaticMaxValueDemo_out.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
