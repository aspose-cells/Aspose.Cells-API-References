##Shape.AlignTopRightCorner
Shape method. Moves the picture to the topright corner
## Shape.AlignTopRightCorner method
Moves the picture to the top-right corner.
```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | the row index. |
| rightColumn | Int32 | the column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape to align
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
// Align the shape's top right corner to row 2, column 5
shape.AlignTopRightCorner(2, 5);
// Save the workbook
workbook.Save("AlignTopRightCornerDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
