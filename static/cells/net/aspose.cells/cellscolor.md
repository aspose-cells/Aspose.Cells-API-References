##Class CellsColor
Aspose.Cells.CellsColor class. Represents all types of color
## CellsColor class
Represents all types of color.
```csharp
public class CellsColor
```
## Properties
| Name | Description |
| --- | --- |
| [Argb](../../aspose.cells/cellscolor/argb/) { get; set; } | Gets and sets the color from a 32-bit ARGB value. |
| [Color](../../aspose.cells/cellscolor/color/) { get; set; } | Gets and sets the RGB color. |
| [ColorIndex](../../aspose.cells/cellscolor/colorindex/) { get; set; } | Gets and sets the color index in the color palette. Only applies of indexed color. |
| [IsShapeColor](../../aspose.cells/cellscolor/isshapecolor/) { get; set; } | Gets and set the color which should apply to cell or shape. |
| [ThemeColor](../../aspose.cells/cellscolor/themecolor/) { get; set; } | Gets the theme color. Only applies for theme color type. |
| [Transparency](../../aspose.cells/cellscolor/transparency/) { get; set; } | Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells/cellscolor/type/) { get; } | The color type. |
## Methods
| Name | Description |
| --- | --- |
| [SetTintOfShapeColor](../../aspose.cells/cellscolor/settintofshapecolor/)(double) | Set the tint of the shape color |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class CellsColorDemo
{
public static void CellsColorExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range of cells
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A10");
// Create a CellsColor instance
CellsColor cellsColor = workbook.CreateCellsColor();
// Set properties of CellsColor
cellsColor.IsShapeColor = false;
cellsColor.Color = Color.Red;
cellsColor.ColorIndex = 5;
cellsColor.Argb = Color.Blue.ToArgb();
cellsColor.Transparency = 0.5;
// Apply the CellsColor to the range
Style style = workbook.CreateStyle();
style.ForegroundColor = cellsColor.Color;
style.Pattern = BackgroundType.Solid;
range.ApplyStyle(style, new StyleFlag { CellShading = true });
// Save the workbook
workbook.Save("CellsColorExample.xlsx");
workbook.Save("CellsColorExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
