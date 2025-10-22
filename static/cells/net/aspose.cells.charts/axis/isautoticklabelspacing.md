##Axis.IsAutoTickLabelSpacing
Axis property. Indicates whether the spacing of tick label is automatic
## Axis.IsAutoTickLabelSpacing property
Indicates whether the spacing of tick label is automatic
```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsAutoTickLabelSpacingDemo
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
valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
// Configure category axis
Axis categoryAxis = chart.CategoryAxis;
categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
categoryAxis.TickLabelSpacing = 2;
workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
