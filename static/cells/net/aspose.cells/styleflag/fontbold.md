##StyleFlag.FontBold
StyleFlag property. Font bold setting will be applied
## StyleFlag.FontBold property
Font bold setting will be applied.
```csharp
public bool FontBold { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyFontBoldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a bold style
Style boldStyle = workbook.CreateStyle();
boldStyle.Font.IsBold = true;
// Apply bold style to row 2 with StyleFlag for FontBold only
worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });
// Put value in cell to demonstrate the style
worksheet.Cells[1, 0].PutValue("Bold Text");
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("FontBold property demo completed successfully.");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
