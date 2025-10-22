##TextParagraph.IsHangingPunctuation
TextParagraph property. Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text
## TextParagraph.IsHangingPunctuation property
Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.
```csharp
public bool IsHangingPunctuation { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyIsHangingPunctuationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet (fixed by adding height parameter)
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";
// Get the text paragraph from the text box (fixed by casting to TextParagraph)
FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
TextParagraph textParagraph = (TextParagraph)fontSetting;
// Display the current value of IsHangingPunctuation
Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);
// Set IsHangingPunctuation to true
textParagraph.IsHangingPunctuation = true;
Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);
// Set IsHangingPunctuation to false
textParagraph.IsHangingPunctuation = false;
Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);
// Save the workbook to see the effects (visual inspection required)
workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
