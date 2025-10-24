##ChartTextFrame.Text
ChartTextFrame property. Gets or sets the text of a frames title
## ChartTextFrame.Text property
Gets or sets the text of a frame's title.
```csharp
public virtual string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyTextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
Cells cells = sheet.Cells;
cells["A1"].PutValue("Category");
cells["A2"].PutValue("A");
cells["A3"].PutValue("B");
cells["A4"].PutValue("C");
cells["B1"].PutValue("Value");
cells["B2"].PutValue(10);
cells["B3"].PutValue(20);
cells["B4"].PutValue(30);
// Add chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Set chart title text
chart.Title.Text = "Sample Chart Title";
// Access and modify legend text
Legend legend = chart.Legend;
legend.Text = "Custom Legend Text";
// Save the workbook
workbook.Save("ChartTextDemo.xlsx");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
