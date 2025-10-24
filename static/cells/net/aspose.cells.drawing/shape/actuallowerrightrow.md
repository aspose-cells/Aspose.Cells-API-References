##Shape.ActualLowerRightRow
Shape property. Get the actual bottom row
## Shape.ActualLowerRightRow property
Get the actual bottom row.
```csharp
public int ActualLowerRightRow { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyActualLowerRightRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape (rectangle)
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);
// Get the actual lower right row of the shape
int actualLowerRightRow = shape.ActualLowerRightRow;
// Output the result
Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
