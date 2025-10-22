##Range.SetOutlineBorders
Range method. Sets the outline borders around a range of cells with same border style and color
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}
Sets the outline borders around a range of cells with same border style and color.
```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | CellsColor | Border color. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodSetOutlineBordersWithCellBorderTypeCellsColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create a CellsColor object with a theme color
CellsColor color = workbook.CreateCellsColor();
color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);
// Create a range and set outline borders
Aspose.Cells.Range range = cells.CreateRange("B2:D5");
range.SetOutlineBorders(CellBorderType.Thin, color);
// Save the workbook
workbook.Save("OutlineBordersDemo.xlsx");
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}
Sets the outline borders around a range of cells with same border style and color.
```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System.Drawing;
public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells (A1:D4)
Range range = worksheet.Cells.CreateRange("A1", "D4");
// Fill the range with some data to make the borders visible
for (int row = 0; row < 4; row++)
{
for (int col = 0; col < 4; col++)
{
worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
}
}
try
{
// Call SetOutlineBorders with medium border style and red color
range.SetOutlineBorders(CellBorderType.Medium, Color.Red);
// Save the workbook to see the effect
workbook.Save("RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}
Sets out line borders around a range of cells.
```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Border styles. |
| borderColors | Color[] | Border colors. |
### Remarks
Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System.Drawing;
public class RangeMethodSetOutlineBordersWithCellBorderTypeColorDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells (B2:D4)
Range range = worksheet.Cells.CreateRange("B2", "D4");
// Prepare border styles and colors
CellBorderType[] borderStyles = new CellBorderType[]
{
CellBorderType.Thick,
CellBorderType.Dashed,
CellBorderType.Double,
CellBorderType.MediumDashDot
};
Color[] borderColors = new Color[]
{
Color.Red,
Color.Blue,
Color.Green,
Color.Purple
};
try
{
// Set outline borders with different styles and colors
range.SetOutlineBorders(borderStyles, borderColors);
// Fill cells with data to make borders visible
for (int row = 1; row <= 3; row++)
{
for (int col = 1; col <= 3; col++)
{
worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
}
}
// Save the workbook
workbook.Save("RangeSetOutlineBordersDemo.xlsx");
}
catch (System.Exception ex)
{
System.Console.WriteLine($"Error executing SetOutlineBorders method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
