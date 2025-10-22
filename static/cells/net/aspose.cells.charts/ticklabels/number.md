##TickLabels.Number
TickLabels property. Represents the format number for the TickLabels object
## TickLabels.Number property
Represents the format number for the TickLabels object.
```csharp
public int Number { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Configure tick labels
TickLabels tickLabels = chart.ValueAxis.TickLabels;
tickLabels.Number = 2; // Demonstrate Number property
tickLabels.NumberFormat = "0.00";
// Save the workbook
workbook.Save("TickLabelsNumberDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
