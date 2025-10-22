##Enum FontFileFormatType
Aspose.Cells.FontFileFormatType enum. Represents font format type
## FontFileFormatType enumeration
Represents font format type.
```csharp
public enum FontFileFormatType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Unknown | `0` | Unknown font format type. |
| Ttf | `1` | TTF font format type. |
| Otf | `2` | OTF font format type. |
| Ttc | `3` | TTC font format type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsClassFontFileFormatTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access a cell and set its style
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Font Format Type Demo");
Style style = cell.GetStyle();
// Demonstrate FontFileFormatType usage
FontFileFormatType fontFormat = FontFileFormatType.Ttf;
Console.WriteLine("Selected font format: " + fontFormat.ToString());
// Apply font settings
style.Font.Name = "Arial";
style.Font.Size = 14;
cell.SetStyle(style);
// Check font format compatibility
if (fontFormat == FontFileFormatType.Ttf)
{
Console.WriteLine("Using TrueType font format");
}
// Save the workbook
workbook.Save("FontFileFormatTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
