##Axis.CrossType
Axis property. Represents the CrossType on the specified axis where the other axis crosses
## Axis.CrossType property
Represents the `CrossType` on the specified axis where the other axis crosses.
```csharp
public CrossType CrossType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyCrossTypeDemo
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
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure value axis
chart.ValueAxis.MaxValue = 200;
chart.ValueAxis.MinValue = 0;
chart.ValueAxis.MajorUnit = 25;
// Demonstrate CrossType property
chart.ValueAxis.CrossType = CrossType.Maximum;
workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
