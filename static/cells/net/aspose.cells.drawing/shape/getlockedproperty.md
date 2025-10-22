##Shape.GetLockedProperty
Shape method. Gets the value of locked property
## Shape.GetLockedProperty method
Gets the value of locked property.
```csharp
public bool GetLockedProperty(ShapeLockType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | The type of the shape locked property. |
### Return Value
Returns the value of locked property.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodGetLockedPropertyWithShapeLockTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Set locked property for AdjustHandles
shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
// Check if AdjustHandles is locked
int noAdjustHandles = 0;
if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
noAdjustHandles = 1;
Console.WriteLine("AdjustHandles locked status: " + (noAdjustHandles == 1));
}
}
}
```
### See Also
* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
