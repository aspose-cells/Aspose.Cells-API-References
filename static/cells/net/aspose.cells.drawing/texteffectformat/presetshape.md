##TextEffectFormat.PresetShape
TextEffectFormat property. Gets and sets the preset shape type
## TextEffectFormat.PresetShape property
Gets and sets the preset shape type.
```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyPresetShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with text effect
Shape shape = worksheet.Shapes.AddTextEffect(
MsoPresetTextEffect.TextEffect1,
"Sample Text",
"Arial",
18,
false,
false,
0,
0,
100,
200,
0,
0);
// Get the text effect format
TextEffectFormat textEffectFormat = shape.TextEffect;
// Set and get PresetShape property
textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);
// Modify other properties
textEffectFormat.Text = "Updated Text";
textEffectFormat.FontBold = true;
textEffectFormat.FontSize = 24;
// Save the workbook
workbook.Save("TextEffectFormatDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
