##Shape.LowerRightColumn
Shape property. Represents lower right corner column index
## Shape.LowerRightColumn property
Represents lower right corner column index.
```csharp
public int LowerRightColumn { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLowerRightColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);
// Set and display the initial LowerRightColumn value
shape.LowerRightColumn = 3;
Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);
// Modify the LowerRightColumn if it equals 3
if (shape.LowerRightColumn == 3)
{
shape.LowerRightColumn = 1;
Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
