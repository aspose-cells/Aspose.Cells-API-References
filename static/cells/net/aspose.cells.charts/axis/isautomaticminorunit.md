##Axis.IsAutomaticMinorUnit
Axis property. Indicates whether the minor unit of the axis is automatically assigned
## Axis.IsAutomaticMinorUnit property
Indicates whether the minor unit of the axis is automatically assigned.
```csharp
public bool IsAutomaticMinorUnit { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsAutomaticMinorUnitDemo
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
chart.SetChartDataRange("A1:B4", true);
// Get the value axis
Axis valueAxis = chart.ValueAxis;
// Demonstrate IsAutomaticMinorUnit property
Console.WriteLine("Initial IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
// Set minor unit manually
valueAxis.IsAutomaticMinorUnit = false;
valueAxis.MinorUnit = 2;
Console.WriteLine("After setting manually - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
Console.WriteLine("MinorUnit: " + valueAxis.MinorUnit);
// Set back to automatic
valueAxis.IsAutomaticMinorUnit = true;
Console.WriteLine("After setting automatic - IsAutomaticMinorUnit: " + valueAxis.IsAutomaticMinorUnit);
// Save the workbook
workbook.Save("AxisPropertyIsAutomaticMinorUnitDemo_out.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
