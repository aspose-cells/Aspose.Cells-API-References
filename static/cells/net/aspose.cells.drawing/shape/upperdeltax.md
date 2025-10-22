##Shape.UpperDeltaX
Shape property. Gets or sets the shapes horizontal offset from its upper left corner column
## Shape.UpperDeltaX property
Gets or sets the shape's horizontal offset from its upper left corner column.
```csharp
public int UpperDeltaX { get; set; }
```
### Remarks
The range of value is 0 to 1024.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyUpperDeltaXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set and display the UpperDeltaX property
shape.UpperDeltaX = 150;
Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);
// Modify the UpperDeltaX if it meets a condition
if (shape.UpperDeltaX == 150)
{
shape.UpperDeltaX = 100;
Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
