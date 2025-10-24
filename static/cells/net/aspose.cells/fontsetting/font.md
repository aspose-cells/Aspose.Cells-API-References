##FontSetting.Font
FontSetting property. Returns the font of this object
## FontSetting.Font property
Returns the font of this object.
```csharp
public Font Font { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontSettingPropertyFontDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample text for font formatting demonstration");
// Apply different font properties to character ranges
cell.Characters(0, 6).Font.IsBold = true;
cell.Characters(7, 4).Font.Color = Color.Blue;
cell.Characters(12, 5).Font.IsItalic = true;
cell.Characters(18, 10).Font.IsStrikeout = true;
cell.Characters(29, 13).Font.Name = "Courier New";
// Save the workbook
workbook.Save("FontSettingDemo.xlsx");
// Verify the saved file
Workbook verifyWorkbook = new Workbook("FontSettingDemo.xlsx");
Cell verifyCell = verifyWorkbook.Worksheets[0].Cells["A1"];
Console.WriteLine("Font formatting applied successfully:");
foreach (FontSetting setting in verifyCell.GetCharacters())
{
Console.WriteLine($"Characters {setting.StartIndex}-{setting.StartIndex + setting.Length - 1}:");
Console.WriteLine($"  Bold: {setting.Font.IsBold}");
Console.WriteLine($"  Italic: {setting.Font.IsItalic}");
Console.WriteLine($"  Strikeout: {setting.Font.IsStrikeout}");
Console.WriteLine($"  Color: {setting.Font.Color}");
Console.WriteLine($"  Font: {setting.Font.Name}");
}
}
}
}
```
### See Also
* class [Font](../../font/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
