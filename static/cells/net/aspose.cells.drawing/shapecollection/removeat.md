##ShapeCollection.RemoveAt
ShapeCollection method. Remove the shape
## ShapeCollection.RemoveAt method
Remove the shape.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the shape. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add first rectangle shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// Add second rectangle shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
// Remove the first shape at index 0
shapes.RemoveAt(0);
// Save the workbook
workbook.Save("ShapeCollectionRemoveAtDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
