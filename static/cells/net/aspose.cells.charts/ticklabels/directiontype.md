##TickLabels.DirectionType
TickLabels property. Gets and sets the direction of text
## TickLabels.DirectionType property
Gets and sets the direction of text.
```csharp
public ChartTextDirectionType DirectionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyDirectionTypeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].Value = 50;
worksheet.Cells["A2"].Value = 100;
worksheet.Cells["A3"].Value = 150;
worksheet.Cells["A4"].Value = 200;
worksheet.Cells["B1"].Value = 60;
worksheet.Cells["B2"].Value = 32;
worksheet.Cells["B3"].Value = 50;
worksheet.Cells["B4"].Value = 40;
worksheet.Cells["C1"].Value = "清华";
worksheet.Cells["C2"].Value = "北大";
worksheet.Cells["C3"].Value = "人大";
worksheet.Cells["C4"].Value = "科大";
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Set tick labels direction to vertical
chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;
// Save the workbook
workbook.Save("TickLabelsDirectionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
