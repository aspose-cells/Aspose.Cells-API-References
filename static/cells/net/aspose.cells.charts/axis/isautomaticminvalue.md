##Axis.IsAutomaticMinValue
Axis property. Indicates whether the min value is automatically assigned
## Axis.IsAutomaticMinValue property
Indicates whether the min value is automatically assigned.
```csharp
public bool IsAutomaticMinValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsAutomaticMinValueDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure value axis
Axis valueAxis = chart.ValueAxis;
valueAxis.IsAutomaticMinValue = false;
valueAxis.MinValue = 0;
valueAxis.IsAutomaticMaxValue = true; // Keep max value automatic for contrast
// Save the result
workbook.Save("AxisPropertyIsAutomaticMinValueDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
