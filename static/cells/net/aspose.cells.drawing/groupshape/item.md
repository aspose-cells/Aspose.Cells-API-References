##GroupShape.Item
GroupShape property. Gets the child shape by index
## GroupShape indexer
Gets the child shape by index.
```csharp
public Shape this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | the child shape index. |
### Return Value
return the child shape.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class GroupShapePropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two rectangle shapes
Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
// Group the shapes
Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);
// Access and display first shape properties
Shape firstShape = groupShape[0];
Console.WriteLine($"First shape initial name: {firstShape.Name}");
Console.WriteLine($"First shape initial text: {firstShape.Text}");
// Modify first shape properties through Item access
firstShape.Name = "ModifiedRectangle1";
firstShape.Text = "First Grouped Shape";
// Access and modify second shape directly through indexer
groupShape[1].Text = "Second Grouped Shape";
// Verify changes
Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");
// Save modified workbook
workbook.Save("GroupShapePropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
