##TextParagraph.FontAlignType
TextParagraph property. Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines
## TextParagraph.FontAlignType property
Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines.
```csharp
public TextFontAlignType FontAlignType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyFontAlignTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.Text = "Sample Text\nFor Font Alignment Demo";
// Get the first paragraph of the text box
TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
// Display the current FontAlignType value
Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);
// Set FontAlignType to Bottom
paragraph.FontAlignType = TextFontAlignType.Bottom;
Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);
// Set FontAlignType to Center
paragraph.FontAlignType = TextFontAlignType.Center;
Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);
// Set FontAlignType to Top
paragraph.FontAlignType = TextFontAlignType.Top;
Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);
// Save the workbook to see the effects
workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
