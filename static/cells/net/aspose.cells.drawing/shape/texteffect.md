##Shape.TextEffect
Shape property. Returns a TextEffectFormat object that contains texteffect formatting properties for the specified shape. Applies to Shape objects that represent WordArt
## Shape.TextEffect property
Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.
```csharp
public TextEffectFormat TextEffect { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a WordArt shape with correct parameters
Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);
// Check if it's WordArt and access TextEffect properties
if (shape.IsWordArt)
{
TextEffectFormat textEffectFormat = shape.TextEffect;
textEffectFormat.FontBold = true;
textEffectFormat.FontItalic = true;
textEffectFormat.FontName = "Arial";
textEffectFormat.FontSize = 14;
}
// Save the workbook
workbook.Save("TextEffectDemo.xlsx");
}
}
}
```
### See Also
* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
