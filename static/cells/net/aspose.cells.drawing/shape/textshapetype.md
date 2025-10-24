##Shape.TextShapeType
Shape property. Gets and sets the preset text shape type
## Shape.TextShapeType property
Gets and sets the preset text shape type.
```csharp
public AutoShapeType TextShapeType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTextShapeTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);
// Check and set TextShapeType if unknown
if (shape.TextShapeType == AutoShapeType.Unknown)
{
shape.TextShapeType = AutoShapeType.Rectangle;
}
// Output the shape's TextShapeType
Console.WriteLine("Shape TextShapeType: " + shape.TextShapeType);
}
}
}
```
### See Also
* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
