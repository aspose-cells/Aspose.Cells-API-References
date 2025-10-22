##StyleFlag.RightBorder
StyleFlag property. Right border settings will be applied
## StyleFlag.RightBorder property
Right border settings will be applied.
```csharp
public bool RightBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyRightBorderDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with borders
Style borderStyle = workbook.CreateStyle();
borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;
// Create style flag and enable right border
StyleFlag borderFlag = new StyleFlag();
borderFlag.RightBorder = true;
// Apply the style to a cell
Cell cell = worksheet.Cells["B2"];
cell.SetStyle(borderStyle, borderFlag);
// Save the workbook
workbook.Save("RightBorderDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
