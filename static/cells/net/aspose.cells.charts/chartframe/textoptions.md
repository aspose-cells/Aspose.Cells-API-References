##ChartFrame.TextOptions
ChartFrame property. Gets and sets the options of the text
## ChartFrame.TextOptions property
Gets and sets the options of the text.
```csharp
public virtual TextOptions TextOptions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyTextOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A2"].PutValue("カテゴリー1");
sheet.Cells["A3"].PutValue("カテゴリー2");
sheet.Cells["A4"].PutValue("カテゴリー3");
sheet.Cells["B1"].PutValue("列 1");
sheet.Cells["B2"].PutValue(4);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(50);
sheet.Cells["C1"].PutValue("列 2");
sheet.Cells["C2"].PutValue(50);
sheet.Cells["C3"].PutValue(100);
sheet.Cells["C4"].PutValue(150);
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = sheet.Charts[chartIndex];
chart.Title.Text = "マーケット";
chart.Title.TextOptions.LanguageCode = CountryCode.Japan;
chart.SetChartDataRange("A1:C4", true);
workbook.Save("ChartTextOptionsOutput.xlsx");
}
}
}
```
### See Also
* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
