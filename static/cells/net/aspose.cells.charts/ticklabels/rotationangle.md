##TickLabels.RotationAngle
TickLabels property. Represents text rotation angle in clockwise
## TickLabels.RotationAngle property
Represents text rotation angle in clockwise.
```csharp
public int RotationAngle { get; set; }
```
### Remarks
0: Not rotated.255: Top to Bottom.-90: Downward.90: Upward.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TickLabelsPropertyRotationAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category 1");
sheet.Cells["A2"].PutValue("Category 2");
sheet.Cells["A3"].PutValue("Category 3");
sheet.Cells["B1"].PutValue(100);
sheet.Cells["B2"].PutValue(200);
sheet.Cells["B3"].PutValue(300);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Rotate category axis tick labels by 45 degrees
chart.CategoryAxis.TickLabels.RotationAngle = 45;
// Save the workbook
workbook.Save("TickLabelsRotationDemo.xlsx");
}
}
}
```
### See Also
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
