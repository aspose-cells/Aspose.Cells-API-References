##ChartTextFrame.ReadingOrder
ChartTextFrame property. Represents text reading order
## ChartTextFrame.ReadingOrder property
Represents text reading order.
```csharp
public TextDirectionType ReadingOrder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyReadingOrderDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
cells["B1"].PutValue("Income");
cells["A2"].PutValue("Company A");
cells["A3"].PutValue("Company B");
cells["A4"].PutValue("Company C");
cells["B2"].PutValue(10000);
cells["B3"].PutValue(20000);
cells["B4"].PutValue(30000);
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 8);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
chart.Title.Text = "Income Analysis";
chart.Title.ReadingOrder = TextDirectionType.RightToLeft;
workbook.Save("ChartReadingOrderDemo.xlsx");
}
}
}
```
### See Also
* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
