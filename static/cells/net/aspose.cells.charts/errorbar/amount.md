##ErrorBar.Amount
ErrorBar property. Represents amount of error bar
## ErrorBar.Amount property
Represents amount of error bar.
```csharp
public double Amount { get; set; }
```
### Remarks
The amount must be greater than or equal to zero.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ErrorBarPropertyAmountDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B1"].PutValue(15);
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["B3"].PutValue(35);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure error bars
foreach (Series series in chart.NSeries)
{
series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
series.YErrorBar.Type = ErrorBarType.FixedValue;
series.YErrorBar.Amount = 5; // Demonstrate Amount property
}
workbook.Save("ErrorBarAmountDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
