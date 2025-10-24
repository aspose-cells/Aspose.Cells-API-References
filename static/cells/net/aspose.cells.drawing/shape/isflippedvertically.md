##Shape.IsFlippedVertically
Shape property. Gets and sets whether shape is vertically flipped
## Shape.IsFlippedVertically property
Gets and sets whether shape is vertically flipped .
```csharp
public bool IsFlippedVertically { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyIsFlippedVerticallyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
Console.WriteLine("Original IsFlippedVertically: " + shape.IsFlippedVertically);
if (shape.IsFlippedVertically == false)
{
shape.IsFlippedVertically = true;
Console.WriteLine("Shape has been flipped vertically");
}
Console.WriteLine("Current IsFlippedVertically: " + shape.IsFlippedVertically);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
