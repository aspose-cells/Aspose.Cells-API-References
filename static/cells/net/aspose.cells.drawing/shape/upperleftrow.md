##Shape.UpperLeftRow
Shape property. Represents the top row index
## Shape.UpperLeftRow property
Represents the top row index.
```csharp
public int UpperLeftRow { get; set; }
```
### Remarks
If the shape is in the shape or in the group , UpperLeftRow will be ignored.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyUpperLeftRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Set and demonstrate UpperLeftRow property
shape.UpperLeftRow = 3;
Console.WriteLine("Shape's initial UpperLeftRow: " + shape.UpperLeftRow);
// Modify the UpperLeftRow based on condition
if (shape.UpperLeftRow == 3)
shape.UpperLeftRow = 1;
Console.WriteLine("Shape's modified UpperLeftRow: " + shape.UpperLeftRow);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
