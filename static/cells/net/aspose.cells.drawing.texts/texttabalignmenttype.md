##Enum TextTabAlignmentType
Aspose.Cells.Drawing.Texts.TextTabAlignmentType enum. Represents the text tab alignment types
## TextTabAlignmentType enumeration
Represents the text tab alignment types.
```csharp
public enum TextTabAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Center | `0` | The text at this tab stop is center aligned. |
| Decimal | `1` | At this tab stop, the decimals are lined up. |
| Left | `2` | The text at this tab stop is left aligned. |
| Right | `3` | The text at this tab stop is right aligned. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextsClassTextTabAlignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a text box to demonstrate tab alignments
int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
var textBox = worksheet.TextBoxes[textBoxIndex];
var paragraph = textBox.TextBody.TextParagraphs[0];
// Add tab stops with different alignment types
paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);
// Set text to demonstrate all alignment types
textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
"Data\tData\tData\t12.34\n" +
"More\tMore\tMore\t56.78";
// Apply formatting to make the tabs visible
textBox.Font.Size = 12;
textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;
// Save the result
workbook.Save("TextTabAlignmentTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
