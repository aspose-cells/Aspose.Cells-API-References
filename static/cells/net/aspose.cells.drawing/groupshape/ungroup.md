##GroupShape.Ungroup
GroupShape method. Ungroups the shape items
## GroupShape.Ungroup method
Ungroups the shape items.
```csharp
public void Ungroup()
```
### Remarks
If the group shape is grouped by another group shape,nothing will be done.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class GroupShapeMethodUngroupDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add two rectangle shapes
Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);
// Group shapes into a GroupShape
GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });
try
{
// Execute Ungroup method
groupShape.Ungroup();
Console.WriteLine("Shapes ungrouped successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error during ungrouping: {ex.Message}");
}
workbook.Save("GroupShapeUngroupDemo.xlsx");
}
}
}
```
### See Also
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
