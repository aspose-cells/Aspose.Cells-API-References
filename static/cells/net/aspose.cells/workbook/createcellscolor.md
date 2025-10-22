##Workbook.CreateCellsColor
Workbook method. Creates a CellsColor object
## Workbook.CreateCellsColor method
Creates a [`CellsColor`](../../cellscolor/) object.
```csharp
public CellsColor CreateCellsColor()
```
### Return Value
Returns a [`CellsColor`](../../cellscolor/) object.
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCreateCellsColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Create a range and set borders with custom color
Aspose.Cells.Range range = workbook.Worksheets[0].Cells.CreateRange("B5:F10");
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
range.SetInsideBorders(BorderType.Horizontal, CellBorderType.Thin, color);
// Verify the border style in a specific cell
Cell cell = workbook.Worksheets[0].Cells["F5"];
Style style = cell.GetStyle();
Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
Console.WriteLine("Top Border: " + style.Borders[BorderType.TopBorder].LineStyle);
Console.WriteLine("Right Border: " + style.Borders[BorderType.RightBorder].LineStyle);
workbook.Save("CreateCellsColorExample.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../../cellscolor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
