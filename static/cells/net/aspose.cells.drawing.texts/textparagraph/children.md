##TextParagraph.Children
TextParagraph property. Gets all text runs in this paragraph. If this paragraph is empty return paragraph itself
## TextParagraph.Children property
Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.
```csharp
public FontSetting[] Children { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyChildrenDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
textBox.Text = "First line\nSecond line\nThird line";
// Get the text paragraph collection
FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
TextParagraph textParagraph = (TextParagraph)fontSetting;
// Display the number of children (text runs) in the paragraph
Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);
// Modify the font settings of each child (text run)
foreach (FontSetting child in textParagraph.Children)
{
child.Font.Size = 12;
child.Font.Color = System.Drawing.Color.Blue;
child.Font.IsBold = true;
}
// Add another line with different formatting
textBox.Text += "\nFourth line";
fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
textParagraph = (TextParagraph)fontSetting;
// Display the updated number of children
Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);
// Save the workbook
workbook.Save("TextParagraphChildrenDemo.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
