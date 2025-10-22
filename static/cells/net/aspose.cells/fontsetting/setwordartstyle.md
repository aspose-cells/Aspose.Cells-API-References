##FontSetting.SetWordArtStyle
FontSetting method. Sets the preset WordArt style
## FontSetting.SetWordArtStyle method
Sets the preset WordArt style.
```csharp
public void SetWordArtStyle(PresetWordArtStyle style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | PresetWordArtStyle | The preset WordArt style. |
### Remarks
Only for the text of shape/chart.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class FontSettingMethodSetWordArtStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some text to cell A1
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text for WordArt");
// Create font setting for the text in cell A1
FontSetting fontSetting = new FontSetting(0, cell.StringValue.Length, workbook.Worksheets);
try
{
// Apply WordArt style to the font setting
fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle3);
Console.WriteLine("WordArt style applied successfully to the text.");
// Show the effect by saving the workbook
worksheet.AutoFitColumn(0);
worksheet.AutoFitRow(0);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetWordArtStyle method: {ex.Message}");
}
// Save the result
workbook.Save("FontSettingMethodSetWordArtStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [PresetWordArtStyle](../../../aspose.cells.drawing/presetwordartstyle/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
