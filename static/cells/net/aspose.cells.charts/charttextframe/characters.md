##ChartTextFrame.Characters
ChartTextFrame method. Returns a Characters object that represents a range of characters within the text
## ChartTextFrame.Characters method
Returns a Characters object that represents a range of characters within the text.
```csharp
public FontSetting Characters(int startIndex, int length)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Int32 | The index of the start of the character. |
| length | Int32 | The number of characters. |
### Return Value
Characters object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFrameMethodCharactersWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Access data labels and set font size for specific characters
chart.NSeries[0].Points[0].DataLabels.ShowValue = true;
chart.NSeries[0].Points[0].DataLabels.Characters(0, 5).Font.Size = 14;
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
