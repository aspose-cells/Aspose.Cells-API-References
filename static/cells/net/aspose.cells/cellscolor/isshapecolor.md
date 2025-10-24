##CellsColor.IsShapeColor
CellsColor property. Gets and set the color which should apply to cell or shape
## CellsColor.IsShapeColor property
Gets and set the color which should apply to cell or shape.
```csharp
public bool IsShapeColor { get; set; }
```
### Remarks
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellsColorPropertyIsShapeColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a CellsColor instance and set IsShapeColor
CellsColor cellsColor = workbook.CreateCellsColor();
cellsColor.IsShapeColor = true;
cellsColor.Color = Color.Green;
// Apply the color to a shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
shape.Fill.FillType = FillType.Solid;
shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly
// Save the workbook
workbook.Save("CellsColorIsShapeColorDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
