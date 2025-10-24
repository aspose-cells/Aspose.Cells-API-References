##Shape.Name
Shape property. Gets and sets the name of the shape
## Shape.Name property
Gets and sets the name of the shape.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set its name
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
shape.Name = "shape1";
// Verify the name was set
Console.WriteLine("Shape name: " + shape.Name);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
