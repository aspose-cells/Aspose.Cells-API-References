##ReflectionEffect.RotWithShape
ReflectionEffect property. Gets and sets if the reflection should rotate with the shape
## ReflectionEffect.RotWithShape property
Gets and sets if the reflection should rotate with the shape.
```csharp
public bool RotWithShape { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ReflectionEffectPropertyRotWithShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Create and apply reflection effect
ReflectionEffect reflection = shape.Reflection;
reflection.Type = ReflectionEffectType.FullReflection4PtOffset;
reflection.Blur = 5;
reflection.Distance = 10;
reflection.Transparency = 0.3;
// Display current RotWithShape value
Console.WriteLine("Current RotWithShape value: " + reflection.RotWithShape);
// Set RotWithShape to true
reflection.RotWithShape = true;
Console.WriteLine("RotWithShape set to: " + reflection.RotWithShape);
// Rotate the shape to demonstrate the effect
shape.RotationAngle = 45;
// Save the workbook
workbook.Save("ReflectionEffectRotWithShapeDemo.xlsx");
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
