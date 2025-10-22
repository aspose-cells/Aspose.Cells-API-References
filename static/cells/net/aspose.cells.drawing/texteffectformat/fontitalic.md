##TextEffectFormat.FontItalic
TextEffectFormat property. Indicates whether font is italic
## TextEffectFormat.FontItalic property
Indicates whether font is italic.
```csharp
public bool FontItalic { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyFontItalicDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text effect
Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text",
"Arial", 18, false, false, 0, 0, 0, 0, 100, 100);
// Get the text effect format
TextEffectFormat textEffectFormat = shape.TextEffect;
// Set FontItalic to true
textEffectFormat.FontItalic = true;
Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);
// Set FontItalic to false
textEffectFormat.FontItalic = false;
Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);
// Save the workbook
workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
