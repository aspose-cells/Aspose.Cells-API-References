##TextEffectFormat.FontName
TextEffectFormat property. The name of the font used in the WordArt
## TextEffectFormat.FontName property
The name of the font used in the WordArt.
```csharp
public string FontName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyFontNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a WordArt shape
Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text",
"Arial", 18, false, false, 0, 0, 0, 0, 100, 100);
// Set and get the FontName property
shape.TextEffect.FontName = "+mn-ea";
string fontName = shape.TextEffect.FontName;
// Output the result
Console.WriteLine("Font Name: " + fontName);
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
