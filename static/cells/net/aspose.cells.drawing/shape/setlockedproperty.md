##Shape.SetLockedProperty
Shape method. Set the locked property
## Shape.SetLockedProperty method
Set the locked property.
```csharp
public void SetLockedProperty(ShapeLockType type, bool value)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | The locked type. |
| value | Boolean | The value of the property. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeMethodSetLockedPropertyWithShapeLockTypeBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
// Demonstrate SetLockedProperty usage
shape.SetLockedProperty(ShapeLockType.AdjustHandles, true);
shape.SetLockedProperty(ShapeLockType.Selection, false);
Console.WriteLine("Shape locked properties set successfully.");
}
}
}
```
### See Also
* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
