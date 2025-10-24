##Shape.Group
Shape property. Gets the group shape which contains this shape
## Shape.Group property
Gets the group shape which contains this shape.
```csharp
public GroupShape Group { get; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyGroupDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create two sample shapes
Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);
// Group the shapes using Shape array parameter
GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });
// Access group through child shape's Group property
GroupShape retrievedGroup = shape1.Group;
// Demonstrate group property usage
retrievedGroup.Name = "MyShapeGroup";
retrievedGroup.Placement = PlacementType.FreeFloating;
workbook.Save("GroupShapeDemo.xlsx");
}
}
}
```
### See Also
* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
