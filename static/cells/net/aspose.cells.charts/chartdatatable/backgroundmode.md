##ChartDataTable.BackgroundMode
ChartDataTable property. Gets and sets the display mode of the background
## ChartDataTable.BackgroundMode property
Gets and sets the display mode of the background
```csharp
public BackgroundMode BackgroundMode { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyBackgroundModeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure data table
chart.ShowDataTable = true;
ChartDataTable chartTable = chart.ChartDataTable;
// Demonstrate BackgroundMode usage
chartTable.BackgroundMode = BackgroundMode.Transparent;
chartTable.Font.Color = Color.Blue;
chartTable.HasBorderOutline = true;
workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
