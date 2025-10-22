##FontSettingCollection.SetWordArtStyle
FontSettingCollection method. Sets the preset WordArt style
## FontSettingCollection.SetWordArtStyle method
Sets the preset WordArt style.
```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt style. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using System;
public class FontSettingCollectionMethodSetWordArtStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a text box to the worksheet
var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
var fontSettingCollection = textBox.TextBody;
// Set initial text
fontSettingCollection.Text = "Sample Text for WordArt Styling";
try
{
// Call SetWordArtStyle method with WordArtStyle7 (Gradient Fill - Blue, Accent 1, Reflection)
fontSettingCollection.SetWordArtStyle(PresetWordArtStyle.WordArtStyle7);
Console.WriteLine("WordArt style applied successfully to the text box.");
// Save the workbook to show the effect
workbook.Save("FontSettingCollectionSetWordArtStyleDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)
