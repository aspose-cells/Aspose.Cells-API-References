##Shape.Placement
Shape property. Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet
## Shape.Placement property
Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.
```csharp
public PlacementType Placement { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyPlacementDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 50);
// Demonstrate Placement property
Console.WriteLine("Original Placement: " + shape.Placement);
// Change placement type
shape.Placement = PlacementType.MoveAndSize;
Console.WriteLine("Modified Placement: " + shape.Placement);
// Save the workbook
workbook.Save("ShapePlacementDemo.xlsx");
}
}
}
```
### See Also
* enum [PlacementType](../../placementtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
