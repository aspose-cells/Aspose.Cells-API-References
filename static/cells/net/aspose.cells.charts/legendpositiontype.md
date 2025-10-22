##Enum LegendPositionType
Aspose.Cells.Charts.LegendPositionType enum. Enumerates the legend position types
## LegendPositionType enumeration
Enumerates the legend position types.
```csharp
public enum LegendPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Bottom | `0` | Displays the legend to the bottom of the chart's plot area. |
| Corner | `1` | Displays the legend to the corner of the chart's plot area. |
| Left | `4` | Displays the legend to the left of the chart's plot area. |
| NotDocked | `7` | Represents that the legend is not docked. |
| Right | `3` | Displays the legend to the right of the chart's plot area. |
| Top | `2` | Displays the legend to the top of the chart's plot area. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class LegendPositionTypeDemo
{
public static void LegendPositionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to the worksheet
Cells cells = sheet.Cells;
cells[0, 1].PutValue("Income");
cells[1, 0].PutValue("Company A");
cells[2, 0].PutValue("Company B");
cells[3, 0].PutValue("Company C");
cells[1, 1].PutValue(10000);
cells[2, 1].PutValue(20000);
cells[3, 1].PutValue(30000);
// Add a column chart to the worksheet
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Access the legend of the chart
Legend legend = chart.Legend;
// Set the legend's position to the left of the chart
legend.Position = LegendPositionType.Left;
// Set additional properties for the legend
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50;
// Save the workbook
workbook.Save("LegendPositionTypeExample.xlsx");
workbook.Save("LegendPositionTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
