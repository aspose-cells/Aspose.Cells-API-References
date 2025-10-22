##Shape.LowerDeltaX
Shape property. Gets or sets the shapes horizontal offset from its lower right corner column
## Shape.LowerDeltaX property
Gets or sets the shape's horizontal offset from its lower right corner column.
```csharp
public int LowerDeltaX { get; set; }
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
public class ShapePropertyLowerDeltaXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and demonstrate LowerDeltaX property
shape.LowerDeltaX = 3;
Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);
// Modify LowerDeltaX if condition is met
if (shape.LowerDeltaX == 3)
{
shape.LowerDeltaX = 1;
Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
