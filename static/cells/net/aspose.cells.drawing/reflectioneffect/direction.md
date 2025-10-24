##ReflectionEffect.Direction
ReflectionEffect property. Gets and sets the direction of the alpha gradient ramp relative to the shape itself
## ReflectionEffect.Direction property
Gets and sets the direction of the alpha gradient ramp relative to the shape itself.
```csharp
public double Direction { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ReflectionEffectPropertyDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to apply reflection effect
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Get the reflection effect of the shape
ReflectionEffect reflection = shape.Reflection;
// Display current Direction value
Console.WriteLine("Current Direction value: " + reflection.Direction);
// Set new Direction value (90 degrees)
reflection.Direction = 90;
Console.WriteLine("New Direction value: " + reflection.Direction);
// Configure other reflection properties for better visibility
reflection.Type = ReflectionEffectType.TightReflectionTouching;
reflection.Transparency = 0.5;
reflection.Size = 50;
reflection.Blur = 5;
// Save the workbook to see the reflection effect
workbook.Save("ReflectionEffectDirectionDemo.xlsx");
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
