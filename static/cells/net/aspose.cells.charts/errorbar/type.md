##ErrorBar.Type
ErrorBar property. Represents error bar amount type
## ErrorBar.Type property
Represents error bar amount type.
```csharp
public ErrorBarType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add sample data
ws.Cells["A1"].PutValue(5);
ws.Cells["A2"].PutValue(3);
// Create a chart
int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = ws.Charts[chartIndex];
// Add series data
chart.NSeries.Add("A3:A10", true);
Series series = chart.NSeries[0];
// Set custom error bar type and values
series.YErrorBar.Type = ErrorBarType.Custom;
series.YErrorBar.PlusValue = "=Sheet1!A1";
series.YErrorBar.MinusValue = "=Sheet1!A2";
// Save the workbook
wb.Save("ErrorBarDemo.xlsx");
}
}
}
```
### See Also
* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
