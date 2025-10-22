##TextParagraph.IsEastAsianLineBreak
TextParagraph property. Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added
## TextParagraph.IsEastAsianLineBreak property
Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.
```csharp
public bool IsEastAsianLineBreak { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyIsEastAsianLineBreakDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";
// Get the text paragraph from the text box's first paragraph
TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
// Display the current value of IsEastAsianLineBreak
Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);
// Set IsEastAsianLineBreak to false (East Asian words can be broken)
paragraph.IsEastAsianLineBreak = false;
Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");
// Save the workbook with East Asian line break disabled
workbook.Save("EastAsianLineBreakDisabled.xlsx");
// Set IsEastAsianLineBreak to true (East Asian words won't be broken)
paragraph.IsEastAsianLineBreak = true;
Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");
// Save the workbook with East Asian line break enabled
workbook.Save("EastAsianLineBreakEnabled.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
