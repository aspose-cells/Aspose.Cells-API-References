##StyleFlag.FontUnderline
StyleFlag property. Font underline setting will be applied
## StyleFlag.FontUnderline property
Font underline setting will be applied.
```csharp
public bool FontUnderline { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyFontUnderlineDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set some text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text with Underline");
// Create a style object and set font underline
Style style = workbook.CreateStyle();
style.Font.Underline = FontUnderlineType.Single;
// Create a style flag and enable font underline flag
StyleFlag styleFlag = new StyleFlag();
styleFlag.FontUnderline = true;
// Apply the style to the cell with the style flag
cell.SetStyle(style, styleFlag);
// Display current underline status
Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);
// Change the underline type to double
style.Font.Underline = FontUnderlineType.Double;
cell.SetStyle(style, styleFlag);
Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);
// Save the workbook
workbook.Save("FontUnderlineDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
