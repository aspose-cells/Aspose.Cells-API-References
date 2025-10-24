##ErrorBar.PlusValue
ErrorBar property. Represents positive error amount when error bar type is Custom
## ErrorBar.PlusValue property
Represents positive error amount when error bar type is Custom.
```csharp
public string PlusValue { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyPlusValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(5);
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(40);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
// Configure error bars
ErrorBar errorBar = chart.NSeries[0].YErrorBar;
errorBar.DisplayType = ErrorBarDisplayType.Both;
errorBar.Type = ErrorBarType.Custom;
errorBar.PlusValue = "=A2";  // Using PlusValue property
errorBar.MinusValue = "=A3";
// Save the workbook
workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
