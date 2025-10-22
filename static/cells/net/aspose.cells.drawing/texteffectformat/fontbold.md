##TextEffectFormat.FontBold
TextEffectFormat property. Indicates whether font is bold
## TextEffectFormat.FontBold property
Indicates whether font is bold.
```csharp
public bool FontBold { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyFontBoldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box shape (returns TextBox object directly)
TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
textbox.Text = "Sample Text";
// Get the text effect format
TextEffectFormat effFormat = textbox.TextEffect;
// Set font properties including bold
effFormat.FontName = "Arial";
effFormat.FontBold = true;
effFormat.FontItalic = false;
effFormat.FontSize = 14;
// Save the workbook
workbook.Save("TextEffectFormatFontBoldDemo.xlsx");
Console.WriteLine("Text effect format with bold font applied successfully.");
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
