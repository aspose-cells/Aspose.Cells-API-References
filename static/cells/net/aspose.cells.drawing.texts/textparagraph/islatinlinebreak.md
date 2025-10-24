##TextParagraph.IsLatinLineBreak
TextParagraph property. Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added
## TextParagraph.IsLatinLineBreak property
Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.
```csharp
public bool IsLatinLineBreak { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class TextParagraphPropertyIsLatinLineBreakDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet (fixed parameters to include height)
TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";
// Get the text paragraph of the text box (added explicit cast)
FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
TextParagraph textParagraph = ((TextParagraph)fontSetting);
// Display the current value of IsLatinLineBreak
Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);
// Set IsLatinLineBreak to false (Latin words won't break at line end)
textParagraph.IsLatinLineBreak = false;
Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
workbook.Save("LatinLineBreakDisabled.xlsx");
// Set IsLatinLineBreak to true (Latin words can break at line end)
textParagraph.IsLatinLineBreak = true;
Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
workbook.Save("LatinLineBreakEnabled.xlsx");
}
}
}
```
### See Also
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
