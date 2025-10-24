##Shape.Type
Shape property. Gets the auto shape type
## Shape.Type property
Gets the auto shape type.
```csharp
public AutoShapeType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);
// Get and display the shape type
AutoShapeType autoShapeType = shape.Type;
Console.WriteLine("Shape Type: " + autoShapeType);
// Cannot change shape type as Type property is read-only
// Instead create a new shape with different type
Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
Console.WriteLine("New Shape Type: " + ovalShape.Type);
}
}
}
```
### See Also
* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
