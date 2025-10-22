##Enum TextFontAlignType
Aspose.Cells.Drawing.Texts.TextFontAlignType enum. Represents the different types of font alignment
## TextFontAlignType enumeration
Represents the different types of font alignment.
```csharp
public enum TextFontAlignType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | When the text flow is horizontal or simple vertical same as fontBaseline but for other vertical modes same as fontCenter. |
| Bottom | `1` | The letters are anchored to the very bottom of a single line. |
| Baseline | `2` | The letters are anchored to the bottom baseline of a single line. |
| Center | `3` | The letters are anchored between the two baselines of a single line. |
| Top | `4` | The letters are anchored to the top baseline of a single line. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextsClassTextFontAlignTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create text boxes with different font alignments
var textBoxAuto = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
textBoxAuto.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Automatic;
textBoxAuto.Text = "Automatic Alignment";
var textBoxBottom = worksheet.Shapes.AddTextBox(0, 200, 100, 100, 200, 200);
textBoxBottom.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Bottom;
textBoxBottom.Text = "Bottom Alignment";
var textBoxBaseline = worksheet.Shapes.AddTextBox(0, 400, 100, 100, 200, 200);
textBoxBaseline.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Baseline;
textBoxBaseline.Text = "Baseline Alignment";
var textBoxCenter = worksheet.Shapes.AddTextBox(200, 0, 100, 100, 200, 200);
textBoxCenter.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Center;
textBoxCenter.Text = "Center Alignment";
var textBoxTop = worksheet.Shapes.AddTextBox(200, 200, 100, 100, 200, 200);
textBoxTop.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Top;
textBoxTop.Text = "Top Alignment";
// Display all enum values in console
Console.WriteLine("TextFontAlignType values:");
Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
Console.WriteLine($"Center: {TextFontAlignType.Center}");
Console.WriteLine($"Top: {TextFontAlignType.Top}");
// Save the workbook
workbook.Save("TextFontAlignTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
