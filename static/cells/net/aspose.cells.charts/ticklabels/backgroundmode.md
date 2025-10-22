##TickLabels.BackgroundMode
TickLabels property. Gets and sets the display mode of the background
## TickLabels.BackgroundMode property
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
public class TickLabelsPropertyBackgroundModeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure tick labels
TickLabels tickLabels = chart.ValueAxis.TickLabels;
tickLabels.BackgroundMode = BackgroundMode.Transparent;
tickLabels.RotationAngle = 45;
workbook.Save("TickLabelsBackgroundModeDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundMode](../../backgroundmode/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
