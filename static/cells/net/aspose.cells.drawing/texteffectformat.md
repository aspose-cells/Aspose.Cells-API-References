##Class TextEffectFormat
Aspose.Cells.Drawing.TextEffectFormat class. Contains properties and methods that apply to WordArt objects
## TextEffectFormat class
Contains properties and methods that apply to WordArt objects.
```csharp
public class TextEffectFormat
```
## Properties
| Name | Description |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Indicates whether font is bold. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Indicates whether font is italic. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | The name of the font used in the WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | The size (in points) of the font used in the WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Gets and sets the preset shape type. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | The text in the WordArt. |
## Methods
| Name | Description |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Sets the preset text effect. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassTextEffectFormatDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.Worksheets[0].Shapes;
// Add text effect shape
shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
// Modify text effect
TextEffectFormat textEffectFormat = shapes[0].TextEffect;
textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
// Save the workbook
workbook.Save("TextEffectDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
