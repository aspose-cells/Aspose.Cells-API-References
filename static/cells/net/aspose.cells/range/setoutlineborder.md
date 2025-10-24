##Range.SetOutlineBorder
Range method. Sets outline border around a range of cells
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}
Sets outline border around a range of cells.
```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle,
CellsColor borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Border edge. |
| borderStyle | CellBorderType | Border style. |
| borderColor | CellsColor | Border color. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeCellsCDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a CellsColor object
CellsColor color = workbook.CreateCellsColor();
color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);
// Create a range and set right border
Aspose.Cells.Range range = cells.CreateRange("A2:B3");
range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);
// Create another range and set all borders
range = cells.CreateRange("C6:F10");
range.SetOutlineBorders(CellBorderType.Thin, color);
// Save the workbook
workbook.Save("SetOutlineBorderExample.xlsx");
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
## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}
Sets outline border around a range of cells.
```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Border edge. |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodSetOutlineBorderWithBorderTypeCellBorderTypeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:D5");
// Set outline borders with different border types and colors
range.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Medium, Color.Blue);
range.SetOutlineBorder(BorderType.TopBorder, CellBorderType.Dashed, Color.Green);
range.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);
// Save the workbook
workbook.Save("RangeOutlineBorderDemo.xlsx");
}
}
}
```
### See Also
* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
