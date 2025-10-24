##RenderingFont.Italic
RenderingFont property. Gets or sets italic for the font
## RenderingFont.Italic property
Gets or sets italic for the font.
```csharp
public bool Italic { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingFontPropertyItalicDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a RenderingFont with Italic property set
RenderingFont renderingFont = new RenderingFont("Arial", 16)
{
Italic = true,
Color = Color.Red
};
// Apply the font to cell A1
sheet.Cells["A1"].PutValue("Italic Text Example");
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";  // Directly use the font name
style.Font.Size = (int)renderingFont.Size;  // Explicit cast to int
style.Font.IsItalic = renderingFont.Italic;
style.Font.Color = renderingFont.Color;
sheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("ItalicFontExample.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
