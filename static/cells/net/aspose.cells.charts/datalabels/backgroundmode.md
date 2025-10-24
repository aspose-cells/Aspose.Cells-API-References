##DataLabels.BackgroundMode
DataLabels property. Gets and sets the display mode of the background
## DataLabels.BackgroundMode property
Gets and sets the display mode of the background
```csharp
public BackgroundMode BackgroundMode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DataLabelsPropertyBackgroundModeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(5);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", true);
// Get data labels
Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
dataLabels.ShowValue = true;
// Demonstrate BackgroundMode property
dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
Console.WriteLine("BackgroundMode set to Automatic");
// Save the workbook
workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
