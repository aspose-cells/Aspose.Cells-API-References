##FontSetting.Type
FontSetting property. Gets the type of text node
## FontSetting.Type property
Gets the type of text node.
```csharp
public virtual TextNodeType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;  // Added this using directive
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add text to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
// Get font settings for the cell's characters
FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);
// Display the current Type value
Console.WriteLine("Current Type value: " + fontSetting.Type);
// Demonstrate how Type affects text processing
if (fontSetting.Type == TextNodeType.TextRun)
{
Console.WriteLine("The text is a standard text run.");
}
else if (fontSetting.Type == TextNodeType.TextParagraph)
{
Console.WriteLine("The text is part of a paragraph.");
}
else if (fontSetting.Type == TextNodeType.Equation)
{
Console.WriteLine("The text represents an equation.");
}
// Apply different formatting based on Type
if (fontSetting.Type == TextNodeType.TextRun)
{
fontSetting.Font.Color = System.Drawing.Color.Red;
fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
}
// Save the result
workbook.Save("FontSettingTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
