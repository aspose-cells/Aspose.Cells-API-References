##TextParagraph.FirstLineIndent
TextParagraph property. Specifies the indent size that will be applied to the first line of text in the paragraph
## TextParagraph.FirstLineIndent property
Specifies the indent size that will be applied to the first line of text in the paragraph.
```csharp
public double FirstLineIndent { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyFirstLineIndentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";
// Get the text paragraph from the text box
FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
TextParagraph textParagraph = (TextParagraph)fontSetting;
// Display current FirstLineIndent value
Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);
// Set a new FirstLineIndent value (20 points)
textParagraph.FirstLineIndent = 20;
Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);
// Add another text box to compare with default indent
TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";
// Save the workbook to see the effects
workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
