##ChartCalculateOptions.ChartCalculateOptions
ChartCalculateOptions constructor. Creates the options for calculating chart
## ChartCalculateOptions constructor
Creates the options for calculating chart.
```csharp
public ChartCalculateOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartCalculateOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Create ChartCalculateOptions using constructor
ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
calculateOptions.UpdateAllPoints = true;
// Recalculate chart with options
chart.Calculate(calculateOptions);
// Save the workbook
workbook.Save("ChartCalculateOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
