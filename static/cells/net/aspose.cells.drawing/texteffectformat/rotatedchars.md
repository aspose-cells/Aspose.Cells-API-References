##TextEffectFormat.RotatedChars
TextEffectFormat property. If truecharacters in the specified WordArt are rotated 90 degrees relative to the WordArts bounding shape
## TextEffectFormat.RotatedChars property
If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape.
```csharp
public bool RotatedChars { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyRotatedCharsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text effect
Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text",
"Arial", 18, false, false, 0, 0, 100, 100, 200, 50);
// Get the text effect format
TextEffectFormat textEffectFormat = shape.TextEffect;
// Set RotatedChars property to true
textEffectFormat.RotatedChars = true;
// Save the workbook
workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");
// Verify the RotatedChars property
Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
