##Shape.Paths
Shape property. Gets the paths of a custom geometric shape
## Shape.Paths property
Gets the paths of a custom geometric shape.
```csharp
public ShapePathCollection Paths { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyPathsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom shape (rectangle) with correct parameters
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 1, 1, 100, 150);
// Check if the shape has custom geometry paths
if (shape.Paths != null)
{
Console.WriteLine("Shape has custom geometry paths:");
Console.WriteLine($"Number of paths: {shape.Paths.Count}");
// Add a new path to the shape's geometry
int newPathIndex = shape.Paths.Add();
Console.WriteLine($"Added new path at index: {newPathIndex}");
}
else
{
Console.WriteLine("No custom geometry path.");
}
}
}
}
```
### See Also
* class [ShapePathCollection](../../shapepathcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
