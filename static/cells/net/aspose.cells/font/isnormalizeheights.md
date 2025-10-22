##Font.IsNormalizeHeights
Font property. Indicates whether the normalization of height that is to be applied to the text run
## Font.IsNormalizeHeights property
Indicates whether the normalization of height that is to be applied to the text run.
```csharp
public bool IsNormalizeHeights { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FontPropertyIsNormalizeHeightsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();
Font font = style.Font;
// Set IsNormalizeHeights property
font.IsNormalizeHeights = true;
Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
cell.PutValue("Test Text");
// Verify the property
Font cellFont = cell.GetStyle().Font;
Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
// Modify the property
cellFont.IsNormalizeHeights = false;
Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
}
}
}
```
### See Also
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
