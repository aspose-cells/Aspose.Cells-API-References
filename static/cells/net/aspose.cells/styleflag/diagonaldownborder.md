##StyleFlag.DiagonalDownBorder
StyleFlag property. Diagonal down border settings will be applied
## StyleFlag.DiagonalDownBorder property
Diagonal down border settings will be applied.
```csharp
public bool DiagonalDownBorder { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class StyleFlagPropertyDiagonalDownBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access cell A1 and set some text
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Diagonal Down Border Demo");
// Create a style object and set diagonal down border
Style style = workbook.CreateStyle();
style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thick;
style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 0, 255);
// Create a style flag and enable diagonal down border flag
StyleFlag styleFlag = new StyleFlag();
styleFlag.DiagonalDownBorder = true;
// Apply the style with the flag to the cell
cell.SetStyle(style, styleFlag);
// Check if diagonal down border flag is enabled
Console.WriteLine("DiagonalDownBorder flag is enabled: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);
// Disable the diagonal down border flag
styleFlag.DiagonalDownBorder = false;
style.Borders[BorderType.DiagonalDown].LineStyle = CellBorderType.Thin;
style.Borders[BorderType.DiagonalDown].Color = Color.FromArgb(255, 0, 255, 0);
// Apply the style with the flag to the cell
cell.SetStyle(style, styleFlag);
Console.WriteLine("DiagonalDownBorder flag is now: " + cell.GetStyle().Borders[BorderType.DiagonalDown].LineStyle);
// Save the workbook
workbook.Save("StyleFlagPropertyDiagonalDownBorderDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
