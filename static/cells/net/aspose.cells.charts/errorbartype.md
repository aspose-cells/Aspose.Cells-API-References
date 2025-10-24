##Enum ErrorBarType
Aspose.Cells.Charts.ErrorBarType enum. Represents error bar amount type
## ErrorBarType enumeration
Represents error bar amount type.
```csharp
public enum ErrorBarType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Custom | `0` | InnerCustom value type. |
| FixedValue | `1` | Fixed value type. |
| Percent | `2` | Percentage type |
| StDev | `3` | Standard deviation type. |
| StError | `4` | Standard error type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ErrorBarTypeDemo
{
public static void ErrorBarTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Add some sample data
cells["A1"].PutValue(2);
cells["A2"].PutValue(5);
cells["A3"].PutValue(3);
cells["A4"].PutValue(6);
cells["B1"].PutValue(4);
cells["B2"].PutValue(3);
cells["B3"].PutValue(6);
cells["B4"].PutValue(7);
cells["C1"].PutValue("Q1");
cells["C2"].PutValue("Q2");
cells["C3"].PutValue("Y1");
cells["C4"].PutValue("Y2");
// Add a chart to the worksheet
int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
Chart chart = workbook.Worksheets[0].Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Set error bar properties for each series in the chart
for (int i = 0; i < chart.NSeries.Count; i++)
{
Series series = chart.NSeries[i];
series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
series.YErrorBar.Type = ErrorBarType.FixedValue;
series.YErrorBar.Amount = 5;
}
// Save the workbook
workbook.Save("ErrorBarTypeExample.xlsx");
workbook.Save("ErrorBarTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
