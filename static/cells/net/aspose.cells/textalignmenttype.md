##Enum TextAlignmentType
Aspose.Cells.TextAlignmentType enum. Enumerates text alignment types
## TextAlignmentType enumeration
Enumerates text alignment types.
```csharp
public enum TextAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| General | `1792` | Represents general text alignment. |
| Bottom | `528` | Represents bottom text alignment. |
| Center | `1802` | Represents center text alignment. |
| CenterAcross | `1286` | Represents center across text alignment. |
| Distributed | `807` | Represents distributed text alignment. |
| Fill | `1284` | Represents fill text alignment. |
| Justify | `1821` | Represents justify text alignment. |
| Left | `257` | Represents left text alignment. |
| Right | `259` | Represents right text alignment. |
| Top | `512` | Represents top text alignment. |
| JustifiedLow | `832` | Aligns the text with an adjusted kashida length for Arabic text. |
| ThaiDistributed | `896` | Distributes Thai text specially, because each character is treated as a word. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TextAlignmentTypeDemo
{
public static void TextAlignmentTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("Doe");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["B2"].PutValue(85);
worksheet.Cells["B3"].PutValue(90);
worksheet.Cells["B4"].PutValue(78);
// Add a comment to a cell
Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
comment.Note = "This is a comment.";
comment.TextHorizontalAlignment = TextAlignmentType.Center;
comment.TextVerticalAlignment = TextAlignmentType.Top;
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Customize the chart title
chart.Title.Text = "Scores Chart";
chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
chart.Title.TextVerticalAlignment = TextAlignmentType.Top;
// Save the workbook
workbook.Save("TextAlignmentTypeExample.xlsx");
// Output the results
Console.WriteLine("Workbook saved successfully with text alignment settings.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
