##Axis.IsDisplayUnitLabelShown
Axis property. Represents if the display unit label is shown on the specified axis
## Axis.IsDisplayUnitLabelShown property
Represents if the display unit label is shown on the specified axis.
```csharp
public bool IsDisplayUnitLabelShown { get; set; }
```
### Remarks
The default value is True.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsDisplayUnitLabelShownDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue(500000);
worksheet.Cells["A2"].PutValue(1000000);
worksheet.Cells["A3"].PutValue(1500000);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure display unit and label visibility
chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
chart.ValueAxis.IsDisplayUnitLabelShown = true;
workbook.Save("AxisPropertyIsDisplayUnitLabelShownDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
