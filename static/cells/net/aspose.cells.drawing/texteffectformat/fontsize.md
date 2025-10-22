##TextEffectFormat.FontSize
TextEffectFormat property. The size in points of the font used in the WordArt
## TextEffectFormat.FontSize property
The size (in points) of the font used in the WordArt.
```csharp
public int FontSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyFontSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
int textboxIndex = worksheet.TextBoxes.Add(5, 5, 200, 100);
Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[textboxIndex];
// Set text and format
textBox.Text = "Sample Text Effect";
// Get the text effect format
Shape shape = textBox;
TextEffectFormat effectFormat = shape.TextEffect;
// Set font properties including FontSize
effectFormat.FontName = "Arial";
effectFormat.FontBold = true;
effectFormat.FontItalic = false;
effectFormat.FontSize = 18; // Demonstrating FontSize property
// Save the workbook
workbook.Save("TextEffectFontSizeDemo.xlsx");
Console.WriteLine("Text effect with font size 18 created successfully.");
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
