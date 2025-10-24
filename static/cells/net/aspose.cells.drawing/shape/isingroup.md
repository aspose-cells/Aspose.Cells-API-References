##Shape.IsInGroup
Shape property. Indicates whether the shape is grouped
## Shape.IsInGroup property
Indicates whether the shape is grouped.
```csharp
public bool IsInGroup { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapePropertyIsInGroupDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some shapes with all required parameters (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);
// Group the shapes with correct parameters
GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });
// Check if shapes are in group
Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);
// Add an ungrouped shape
Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);
// Save the result
workbook.Save("ShapePropertyIsInGroupDemo.xlsx");
// Ungroup the shapes and get the ungrouped shapes from the group
group.Ungroup();
Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);
// Save the result
workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
