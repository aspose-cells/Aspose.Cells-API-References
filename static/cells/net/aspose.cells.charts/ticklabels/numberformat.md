##TickLabels.NumberFormat
TickLabels property. Represents the format string for the TickLabels object
## TickLabels.NumberFormat property
Represents the format string for the TickLabels object.
```csharp
public string NumberFormat { get; set; }
```
### Remarks
The formatting string is same as a custom format string setting to a cell. For example, "$0".
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyNumberFormatDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(1.2345);
worksheet.Cells["A3"].PutValue(2.3456);
worksheet.Cells["A4"].PutValue(3.4567);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A2:A4", true);
// Set number format for value axis tick labels
chart.ValueAxis.TickLabels.NumberFormat = "0.00";
// Save the workbook
workbook.Save("TickLabelsNumberFormatDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
