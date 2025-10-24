##ErrorBar.MinusValue
ErrorBar property. Represents negative error amount when error bar type is Custom
## ErrorBar.MinusValue property
Represents negative error amount when error bar type is Custom.
```csharp
public string MinusValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyMinusValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Values");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(5);
worksheet.Cells["B1"].PutValue("Data");
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(15);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("B2:B3", true);
// Configure error bars
ErrorBar errorBar = chart.NSeries[0].YErrorBar;
errorBar.DisplayType = ErrorBarDisplayType.Both;
errorBar.Type = ErrorBarType.Custom;
errorBar.PlusValue = "=A2";
errorBar.MinusValue = "=A3";
// Save the workbook
workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
