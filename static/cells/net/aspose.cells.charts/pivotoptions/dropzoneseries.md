##PivotOptions.DropZoneSeries
PivotOptions property. Specifies whether a control for each PivotTable field on the PivotTable column axis of the source PivotTable appears on the chart when dropZonesVisible is set to true
## PivotOptions.DropZoneSeries property
Specifies whether a control for each PivotTable field on the PivotTable column axis of the source PivotTable appears on the chart when dropZonesVisible is set to true.
```csharp
public bool DropZoneSeries { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class PivotOptionsPropertyDropZoneSeriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and get the first sheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Fruit");
sheet.Cells["B1"].PutValue("Quantity");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue("Orange");
sheet.Cells["B3"].PutValue(5);
sheet.Cells["A4"].PutValue("Banana");
sheet.Cells["B4"].PutValue(7);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:B4", true);
// Get pivot options from the chart
PivotOptions options = chart.PivotOptions;
// Demonstrate DropZoneSeries property
Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
options.DropZoneSeries = true;
Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
// Save the workbook
workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
}
}
}
```
### See Also
* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
