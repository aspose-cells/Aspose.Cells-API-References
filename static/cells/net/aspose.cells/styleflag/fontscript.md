##StyleFlag.FontScript
StyleFlag property. Font script setting will be applied
## StyleFlag.FontScript property
Font script setting will be applied.
```csharp
public bool FontScript { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleFlagPropertyFontScriptDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set some text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Sample Text");
// Create a style object and set font script to subscript
Style style = workbook.CreateStyle();
style.Font.IsSubscript = true;
// Create a style flag and enable FontScript flag
StyleFlag styleFlag = new StyleFlag();
styleFlag.FontScript = true;
// Apply the style to the cell with the style flag
cell.SetStyle(style, styleFlag);
// Display the current font script status
Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);
// Change font script to superscript
style.Font.IsSubscript = false;
style.Font.IsSuperscript = false;
cell.SetStyle(style, styleFlag);
// Display the updated font script status
Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);
// Save the workbook
workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
