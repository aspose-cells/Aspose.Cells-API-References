##Cell.SetCharacters
Cell method. Sets rich text format of the cell
## Cell.SetCharacters method
Sets rich text format of the cell.
```csharp
public void SetCharacters(FontSetting[] characters)
```
| Parameter | Type | Description |
| --- | --- | --- |
| characters | FontSetting[] | All Characters objects. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class CellMethodSetCharactersWithFontSettingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
// Set cell value to apply rich text formatting
cell.Value = "Hello World!";
try
{
// Create font settings for different parts of the text
FontSetting[] fontSettings = new FontSetting[2];
// Format first 5 characters (Hello) as bold red
fontSettings[0] = cell.Characters(0, 5);
fontSettings[0].Font.IsBold = true;
fontSettings[0].Font.Color = Color.Red;
// Format remaining characters ( World!) as italic blue
fontSettings[1] = cell.Characters(5, 7);
fontSettings[1].Font.IsItalic = true;
fontSettings[1].Font.Color = Color.Blue;
// Apply the formatted character settings using SetCharacters
cell.SetCharacters(fontSettings);
Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
}
// Save the result
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
