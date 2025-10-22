##ShapePathCollection.Item
ShapePathCollection property. Gets a creation path
## ShapePathCollection indexer
Gets a creation path.
```csharp
public ShapePath this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
Returns [`ShapePath`](../../shapepath/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePathCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom shape (non-primitive shape) with correct parameters
Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 10, 10, 200, 200, 0, 0);
// Access the ShapePathCollection
ShapePathCollection shapePaths = customShape.Paths;
// Add a new path
int pathIndex = shapePaths.Add();
// Access the path using Item property
ShapePath newPath = shapePaths[pathIndex];
// Output information
Console.WriteLine("Path count: " + shapePaths.Count);
Console.WriteLine("Path segment count: " + newPath.PathSegementList.Count);
// Save the workbook
workbook.Save("ShapePathCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePath](../../shapepath/)
* class [ShapePathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
