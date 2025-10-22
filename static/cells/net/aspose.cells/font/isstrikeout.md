##Font.IsStrikeout
Font property. Gets or sets a value indicating whether the font is single strikeout
## Font.IsStrikeout property
Gets or sets a value indicating whether the font is single strikeout.
```csharp
public bool IsStrikeout { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsStrikeoutDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Method 1: Set strikeout through style directly
Cell cell1 = worksheet.Cells["A1"];
Style style1 = cell1.GetStyle();
style1.Font.IsStrikeout = true;
cell1.SetStyle(style1);
cell1.PutValue("Strikeout Text (Style)");
// Method 2: Set strikeout through HTML
Cell cell2 = worksheet.Cells["A2"];
cell2.HtmlString = "<s>Strikeout Text (HTML)</s>";
// Verify strikeout property
Console.WriteLine("A1 IsStrikeout: " + cell1.GetStyle().Font.IsStrikeout);
Console.WriteLine("A2 IsStrikeout: " + cell2.GetStyle().Font.IsStrikeout);
// Save for verification
workbook.Save("FontStrikeoutDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
