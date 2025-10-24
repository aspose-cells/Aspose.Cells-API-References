##Font.Underline
Font property. Gets or sets the font underline type
## Font.Underline property
Gets or sets the font underline type.
```csharp
public FontUnderlineType Underline { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyUnderlineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Access cell and set underline style
Cell cell = sheet.Cells["A1"];
cell.PutValue("Sample Underlined Text");
// Get the style and modify font properties
Style style = cell.GetStyle();
style.Font.Underline = FontUnderlineType.Single;
cell.SetStyle(style);
// Save the workbook
workbook.Save("FontUnderlineDemo.xlsx");
}
}
}
```
### See Also
* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
