##ErrorBar.DisplayType
ErrorBar property. Represents the display type of error bar
## ErrorBar.DisplayType property
Represents the display type of error bar.
```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyDisplayTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Y");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("A2:A4", true);
chart.NSeries.CategoryData = "B2:B4";
// Set error bar display type
chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;
// Save the workbook
workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
