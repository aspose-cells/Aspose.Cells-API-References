##TextEffectFormat.Text
TextEffectFormat property. The text in the WordArt
## TextEffectFormat.Text property
The text in the WordArt.
```csharp
public string Text { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextEffectFormatPropertyTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add a text effect shape and set its text
Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text",
"Arial", 14, false, false, 0, 0, 0, 0, 100, 100);
// Access and modify the text effect's text property
shape.TextEffect.Text = "Updated Text";
// Verify the text was updated
Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
}
}
}
```
### See Also
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
