##Axis.MajorUnit
Axis property. Represents the major units for the axis
## Axis.MajorUnit property
Represents the major units for the axis.
```csharp
public double MajorUnit { get; set; }
```
### Remarks
The major units must be greater than zero.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyMajorUnitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells["A" + (i + 1)].PutValue("Cat " + i);
worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B11", true);
chart.NSeries.CategoryData = "A2:A11";
// Get the category axis
Axis axis = chart.CategoryAxis;
// Display initial major unit
Console.WriteLine("Initial Major Unit: " + axis.MajorUnit);
// Set new major unit
axis.MajorUnit = 3;
Console.WriteLine("Modified Major Unit: " + axis.MajorUnit);
// Save the workbook
workbook.Save("AxisMajorUnitDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
