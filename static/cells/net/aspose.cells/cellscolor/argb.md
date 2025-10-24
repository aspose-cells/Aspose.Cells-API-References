##CellsColor.Argb
CellsColor property. Gets and sets the color from a 32bit ARGB value
## CellsColor.Argb property
Gets and sets the color from a 32-bit ARGB value.
```csharp
public int Argb { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsColorPropertyArgbDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a range and style
Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A5");
Style style = workbook.CreateStyle();
// Create and configure CellsColor using Argb property
CellsColor cellsColor = workbook.CreateCellsColor();
cellsColor.Argb = Color.FromArgb(128, 0, 0, 255).ToArgb(); // Semi-transparent blue
// Apply the color to the style
style.ForegroundColor = cellsColor.Color;
style.Pattern = BackgroundType.Solid;
// Apply style to range
range.ApplyStyle(style, new StyleFlag { CellShading = true });
// Save the workbook
workbook.Save("CellsColorArgbDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
