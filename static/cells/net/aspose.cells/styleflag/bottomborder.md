##StyleFlag.BottomBorder
StyleFlag property. Bottom border settings will be applied
## StyleFlag.BottomBorder property
Bottom border settings will be applied.
```csharp
public bool BottomBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyBottomBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a style with bottom border settings
Style style = workbook.CreateStyle();
style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
style.Borders[BorderType.BottomBorder].Color = Color.Red;
// Create style flag and enable bottom border modification
StyleFlag styleFlag = new StyleFlag();
styleFlag.BottomBorder = true;
// Apply the style with the flag to cell A1
Cell cell = sheet.Cells["A1"];
cell.PutValue("Cell with bottom border");
cell.SetStyle(style, styleFlag);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
