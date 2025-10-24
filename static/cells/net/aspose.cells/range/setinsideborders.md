##Range.SetInsideBorders
Range method. Set inside borders of the range
## Range.SetInsideBorders method
Set inside borders of the range.
```csharp
public void SetInsideBorders(BorderType borderEdge, CellBorderType lineStyle,
CellsColor borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Inside borde type, only can be Vertical and Horizontal. |
| lineStyle | CellBorderType | The border style. |
| borderColor | CellsColor | The color of the border. |
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RangeMethodSetInsideBordersWithBorderTypeCellBorderTypeCellsCDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and set inside borders
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
range.SetInsideBorders(BorderType.Vertical, CellBorderType.Thin, color);
// Verify the borders in a cell within the range
Cell cell = worksheet.Cells["C6"];
Style style = cell.GetStyle();
Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
workbook.Save("SetInsideBordersExample.xlsx");
}
}
}
```
### See Also
* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
