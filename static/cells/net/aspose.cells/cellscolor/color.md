##CellsColor.Color
CellsColor property. Gets and sets the RGB color
## CellsColor.Color property
Gets and sets the RGB color.
```csharp
public Color Color { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellsColorPropertyColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and set colored borders
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B5:F10");
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Red;
range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical, CellBorderType.Thin, color);
// Verify the border settings in a cell
Cell cell = worksheet.Cells["F5"];
Style style = cell.GetStyle();
Console.WriteLine("Left Border: " + style.Borders[BorderType.LeftBorder].LineStyle);
Console.WriteLine("Bottom Border: " + style.Borders[BorderType.BottomBorder].LineStyle);
// Save the workbook
workbook.Save("CellsColorPropertyColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
