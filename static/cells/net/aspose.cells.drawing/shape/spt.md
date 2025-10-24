##Shape.Spt
Shape property. Specifies an optional number that an application can use to associate the particular shape with a defined shape type
## Shape.Spt property
Specifies an optional number that an application can use to associate the particular shape with a defined shape type.
```csharp
public int Spt { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertySptDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);
// Get and display the Spt property
int spt = shape.Spt;
Console.WriteLine("Shape Spt value: " + spt);
// Create a new oval shape to demonstrate different Spt value
Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
