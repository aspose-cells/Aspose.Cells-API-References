##ShapeCollection.Item
ShapeCollection property. Gets the Shape object at the specific index in the list
## ShapeCollection indexer (1 of 2)
Gets the [`Shape`](../../shape/) object at the specific index in the list.
```csharp
public Shape this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some shapes to the worksheet with correct parameters
worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);
// Get the shape collection
ShapeCollection shapes = worksheet.Shapes;
// Demonstrate Item property by getting the first shape
Shape firstShape = shapes[0];
Console.WriteLine("First shape type: " + firstShape.Type);
// Demonstrate Item property by getting shape by ID
Shape shapeById = shapes[2];
Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## ShapeCollection indexer (2 of 2)
Gets the [`Shape`](../../shape/) object by the name of the shape.
```csharp
public Shape this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the shape. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add shapes to the worksheet
ShapeCollection shapes = worksheet.Shapes;
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
shapes.AddOval(5, 0, 2, 0, 130, 130);
// Access shapes using Item property
Shape rectangle = shapes["Rectangle 1"];
if (rectangle != null)
{
rectangle.FillFormat.ForeColor = System.Drawing.Color.Red;
}
Shape oval = shapes["Oval 2"];
if (oval != null)
{
oval.FillFormat.ForeColor = System.Drawing.Color.Blue;
}
// Save the workbook
workbook.Save("ShapeCollectionDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
