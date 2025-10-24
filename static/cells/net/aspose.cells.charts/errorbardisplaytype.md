##Enum ErrorBarDisplayType
Aspose.Cells.Charts.ErrorBarDisplayType enum. Represents error bar display type
## ErrorBarDisplayType enumeration
Represents error bar display type.
```csharp
public enum ErrorBarDisplayType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Both | `0` | Both |
| Minus | `1` | Minus |
| None | `2` | None |
| Plus | `3` | Plus |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ErrorBarDisplayTypeDemo
{
public static void ErrorBarDisplayTypeExample()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue(2);
worksheet.Cells["A2"].PutValue(5);
worksheet.Cells["A3"].PutValue(3);
worksheet.Cells["A4"].PutValue(6);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(3);
worksheet.Cells["B3"].PutValue(6);
worksheet.Cells["B4"].PutValue(7);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Add a column chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Configure error bars for each series in the chart
foreach (Series series in chart.NSeries)
{
series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
series.YErrorBar.Type = ErrorBarType.FixedValue;
series.YErrorBar.Amount = 5;
}
// Save the workbook
workbook.Save("ErrorBarDisplayTypeExample.xlsx");
workbook.Save("ErrorBarDisplayTypeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
