##ChartFrame.IsInnerMode
ChartFrame property. Indicates whether the size of the plot area size includes the tick marks and the axis labels. False specifies that the size shall determine the size of the plot area the tick marks and the axis labels
## ChartFrame.IsInnerMode property
Indicates whether the size of the plot area size includes the tick marks, and the axis labels. False specifies that the size shall determine the size of the plot area, the tick marks, and the axis labels.
```csharp
public bool IsInnerMode { get; set; }
```
### Remarks
Only for Xlsx file.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartFramePropertyIsInnerModeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access chart frame and demonstrate IsInnerMode
Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
chartFrame.IsInnerMode = true; // Set to use inner mode
// Set some basic properties to show the effect
chartFrame.Border.Color = Color.Blue;
chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
chartFrame.Area.ForegroundColor = Color.LightYellow;
workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
