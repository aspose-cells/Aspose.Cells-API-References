##Shape.IsFlippedHorizontally
Shape property. Gets and sets whether shape is horizontally flipped
## Shape.IsFlippedHorizontally property
Gets and sets whether shape is horizontally flipped .
```csharp
public bool IsFlippedHorizontally { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsFlippedHorizontallyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Check and flip horizontally if not already flipped
if (shape.IsFlippedHorizontally == false)
{
shape.IsFlippedHorizontally = true;
Console.WriteLine("Shape was flipped horizontally");
}
else
{
Console.WriteLine("Shape was already flipped horizontally");
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
