##Enum TextNodeType
Aspose.Cells.Drawing.Texts.TextNodeType enum. Represents the node type
## TextNodeType enumeration
Represents the node type.
```csharp
public enum TextNodeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TextRun | `0` | Represents the text node. |
| TextParagraph | `1` | Represents the text paragraph. |
| Equation | `2` | Represents the equation text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextsClassTextNodeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a textbox and get its text paragraphs
int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
textbox.TextBody.AppendText("Sample text with ");
textbox.TextBody.AppendText("different node types");
// Demonstrate TextNodeType usage
foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
{
foreach (FontSetting portion in paragraph.Children)
{
// Get the text portion using StartIndex and Length
string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
Console.WriteLine("Text: " + portionText);
Console.WriteLine("Node Type: " + portion.Type.ToString());
// Example of checking node type
if (portion.Type == TextNodeType.TextRun)
{
portion.Font.Color = System.Drawing.Color.Red;
}
else if (portion.Type == TextNodeType.Equation)
{
portion.Font.Color = System.Drawing.Color.Blue;
}
}
}
// Save the result
workbook.Save("TextNodeTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)
