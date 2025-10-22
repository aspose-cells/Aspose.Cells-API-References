##Enum DisplayUnitType
Aspose.Cells.Charts.DisplayUnitType enum. Represents the type of display unit of charts axis
## DisplayUnitType enumeration
Represents the type of display unit of chart's axis.
```csharp
public enum DisplayUnitType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Display unit is None. |
| Hundreds | `1` | Specifies the values on the chart shall be divided by 100. |
| Thousands | `2` | Specifies the values on the chart shall be divided by 1,000. |
| TenThousands | `3` | Specifies the values on the chart shall be divided by 10,000. |
| HundredThousands | `4` | Specifies the values on the chart shall be divided by 100,000. |
| Millions | `5` | Specifies the values on the chart shall be divided by 1,000,000. |
| TenMillions | `6` | Specifies the values on the chart shall be divided by 10,000,000. |
| HundredMillions | `7` | Specifies the values on the chart shall be divided by 100,000,000. |
| Billions | `8` | Specifies the values on the chart shall be divided by 1,000,000,000. |
| Trillions | `9` | Specifies the values on the chart shall be divided by 1,000,000,000,000. |
| Percentage | `10` | The values on the chart shall be divided by 0.01. |
| Cust | `11` | specifies a custom value for the display unit. |
| Custom | `12` | specifies a custom value for the display unit. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class DisplayUnitTypeDemo
{
public static void DisplayUnitTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
int sheetIndex = workbook.Worksheets.Add();
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue(500000);
worksheet.Cells["A2"].PutValue(1000000);
worksheet.Cells["A3"].PutValue(1500000);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Set the display unit of the value axis to Millions
chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
// Optionally, show the display unit label
chart.ValueAxis.IsDisplayUnitLabelShown = true;
// Save the workbook
workbook.Save("DisplayUnitTypeExample.xlsx");
workbook.Save("DisplayUnitTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
