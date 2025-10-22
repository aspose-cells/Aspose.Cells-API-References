##TickLabels.NumberFormatLinked
TickLabels property. True if the number format is linked to the cells so that the number format changes in the labels when it changes in the cells
## TickLabels.NumberFormatLinked property
True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).
```csharp
public bool NumberFormatLinked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyNumberFormatLinkedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(100);
worksheet.Cells["A2"].PutValue(200);
worksheet.Cells["A3"].PutValue(300);
worksheet.Cells["A4"].PutValue(400);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A1:A4", true);
// Access value axis tick labels
Aspose.Cells.Charts.TickLabels tickLabels = chart.ValueAxis.TickLabels;
// Demonstrate NumberFormatLinked property
Console.WriteLine("NumberFormatLinked (default): " + tickLabels.NumberFormatLinked);
// Change the property
tickLabels.NumberFormatLinked = false;
Console.WriteLine("NumberFormatLinked after change: " + tickLabels.NumberFormatLinked);
// Save the workbook
workbook.Save("TickLabelsNumberFormatLinkedDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
