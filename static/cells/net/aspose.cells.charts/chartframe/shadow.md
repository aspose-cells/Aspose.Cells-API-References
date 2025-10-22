##ChartFrame.Shadow
ChartFrame property. True if the frame has a shadow
## ChartFrame.Shadow property
True if the frame has a shadow.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyShadowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
cells["A1"].PutValue("Category");
cells["A2"].PutValue("A");
cells["A3"].PutValue("B");
cells["A4"].PutValue("C");
cells["B1"].PutValue("Value");
cells["B2"].PutValue(10);
cells["B3"].PutValue(20);
cells["B4"].PutValue(30);
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
Legend legend = chart.Legend;
legend.Shadow = true;
legend.Position = LegendPositionType.Bottom;
chart.Title.Text = "Shadow Property Demo";
chart.Title.Shadow = true;
workbook.Save("ChartFrameShadowDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
