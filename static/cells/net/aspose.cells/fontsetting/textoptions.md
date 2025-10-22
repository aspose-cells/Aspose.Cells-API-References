##FontSetting.TextOptions
FontSetting property. Returns the text options
## FontSetting.TextOptions property
Returns the text options.
```csharp
public TextOptions TextOptions { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontSettingPropertyTextOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample text with different formatting sections
string part1 = "This is normal text. ";
string part2 = "This is bold and italic text. ";
string part3 = "This is normal again. ";
string part4 = "This is bold text.";
// Combine all parts into one cell
Cell cell = worksheet.Cells["A1"];
cell.Value = part1 + part2 + part3 + part4;
// Apply formatting to specific parts of the text
int startPos1 = part1.Length;
int length1 = part2.Length;
cell.Characters(startPos1, length1).TextOptions.IsBold = true;
cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
int startPos2 = part1.Length + part2.Length + part3.Length;
int length2 = part4.Length;
cell.Characters(startPos2, length2).TextOptions.IsBold = true;
// Save the workbook
workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("TextOptions demo completed. File saved.");
}
}
}
```
### See Also
* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
