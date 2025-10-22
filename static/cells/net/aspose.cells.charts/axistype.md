##Enum AxisType
Aspose.Cells.Charts.AxisType enum. Represents the axis type
## AxisType enumeration
Represents the axis type.
```csharp
public enum AxisType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Category | `0` | Category axis |
| Value | `1` | Value axis |
| Series | `2` | Series axis |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class AxisTypeDemo
{
public static void AxisTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Determine which axes exist in the chart
bool hasPrimaryCategoryAxis = chart.HasAxis(AxisType.Category, true);
bool hasSecondaryCategoryAxis = chart.HasAxis(AxisType.Category, false);
bool hasPrimaryValueAxis = chart.HasAxis(AxisType.Value, true);
bool hasSecondaryValueAxis = chart.HasAxis(AxisType.Value, false);
// Output the results
Console.WriteLine("Has Primary Category Axis: " + hasPrimaryCategoryAxis);
Console.WriteLine("Has Secondary Category Axis: " + hasSecondaryCategoryAxis);
Console.WriteLine("Has Primary Value Axis: " + hasPrimaryValueAxis);
Console.WriteLine("Has Secondary Value Axis: " + hasSecondaryValueAxis);
// Save the workbook
workbook.Save("AxisTypeExample.xlsx");
workbook.Save("AxisTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
