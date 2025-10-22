##GroupShape.GetGroupedShapes
GroupShape method. Gets the shapes grouped by this shape
## GroupShape.GetGroupedShapes method
Gets the shapes grouped by this shape.
```csharp
public Shape[] GetGroupedShapes()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class GroupShapeMethodGetGroupedShapesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 50, 60);
shape1.AlternativeText = "Rectangle1";
Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddOval(2, 0, 50, 100, 50, 60);
shape2.AlternativeText = "Oval1";
Aspose.Cells.Drawing.GroupShape groupShape = worksheet.Shapes.Group(new Aspose.Cells.Drawing.Shape[] { shape1, shape2 });
Aspose.Cells.Drawing.Shape[] groupedShapes = groupShape.GetGroupedShapes();
Console.WriteLine("Group contains " + groupedShapes.Length + " shapes:");
foreach (Aspose.Cells.Drawing.Shape shape in groupedShapes)
{
Console.WriteLine($"Type: {shape.Type}, AltText: {shape.AlternativeText}");
}
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
