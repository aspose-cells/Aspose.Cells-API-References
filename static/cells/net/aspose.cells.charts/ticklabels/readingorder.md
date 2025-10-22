##TickLabels.ReadingOrder
TickLabels property. Represents text reading order
## TickLabels.ReadingOrder property
Represents text reading order.
```csharp
public TextDirectionType ReadingOrder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyReadingOrderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A3", true);
// Set tick labels reading order
TickLabels tickLabels = chart.ValueAxis.TickLabels;
tickLabels.ReadingOrder = TextDirectionType.RightToLeft;
// Save the workbook
workbook.Save("TickLabelsReadingOrderDemo.xlsx");
}
}
}
```
### See Also
* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
