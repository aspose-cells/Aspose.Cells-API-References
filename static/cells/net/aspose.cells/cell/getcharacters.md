##Cell.GetCharacters
Cell method. Returns all Characters objects that represents a range of characters within the cell text
## GetCharacters() {#getcharacters}
Returns all Characters objects that represents a range of characters within the cell text.
```csharp
public FontSetting[] GetCharacters()
```
### Return Value
All Characters objects
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetCharactersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set HTML formatted text in cell A1 with different formatting parts
worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";
// Get the character formatting information from cell A1
FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();
// Output the formatting information
Console.WriteLine("Character formatting in cell A1:");
for (int i = 0; i < fontSettings.Length; i++)
{
Console.WriteLine($"Part {i + 1}:");
Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
Console.WriteLine($"Length: {fontSettings[i].Length}");
Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
Console.WriteLine();
}
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetCharacters(bool) {#getcharacters_1}
Returns all Characters objects that represents a range of characters within the cell text.
```csharp
public FontSetting[] GetCharacters(bool flag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| flag | Boolean | Indicates whether applying table style to the cell if the cell is in the table. |
### Return Value
All Characters objects
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellMethodGetCharactersWithBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add text to cell C8 with formatting
Cell cell = worksheet.Cells["C8"];
cell.PutValue("Formatted Text");
// Format portions of the text
FontSetting fs1 = cell.Characters(0, 8);
fs1.Font.Color = System.Drawing.Color.White;
FontSetting fs2 = cell.Characters(9, 4);
fs2.Font.Color = System.Drawing.Color.Blue;
// Get all font settings with formatting
FontSetting[] fontSettings = cell.GetCharacters(true);
// Display font colors
Console.WriteLine("Font colors in cell C8:");
foreach (FontSetting fs in fontSettings)
{
Console.WriteLine(fs.Font.Color);
}
}
}
}
```
### See Also
* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
