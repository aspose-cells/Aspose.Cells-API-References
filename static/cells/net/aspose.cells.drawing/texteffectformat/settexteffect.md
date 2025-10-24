##TextEffectFormat.SetTextEffect
TextEffectFormat method. Sets the preset text effect
## TextEffectFormat.SetTextEffect method
Sets the preset text effect.
```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```
| Parameter | Type | Description |
| --- | --- | --- |
| effect | MsoPresetTextEffect | The preset text effect. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape for WordArt
Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);
// Get the TextEffectFormat of the shape
TextEffectFormat textEffectFormat = wordArt.TextEffect;
try
{
// Call the SetTextEffect method with MsoPresetTextEffect parameter
textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
// Set additional properties for the WordArt
textEffectFormat.FontBold = true;
textEffectFormat.FontItalic = false;
textEffectFormat.FontSize = 24;
Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
}
// Save the result
workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
