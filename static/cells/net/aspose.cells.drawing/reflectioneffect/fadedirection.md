##ReflectionEffect.FadeDirection
ReflectionEffect property. Gets and sets the direction to offset the reflection
## ReflectionEffect.FadeDirection property
Gets and sets the direction to offset the reflection.
```csharp
public double FadeDirection { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ReflectionEffectPropertyFadeDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to apply reflection effect
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Get the reflection effect of the shape
ReflectionEffect reflection = shape.Reflection;
// Display current FadeDirection value
Console.WriteLine("Current FadeDirection value: " + reflection.FadeDirection);
// Set new FadeDirection value (90 degrees)
reflection.FadeDirection = 90;
Console.WriteLine("New FadeDirection value: " + reflection.FadeDirection);
// Configure other reflection properties for better visibility
reflection.Type = ReflectionEffectType.TightReflectionTouching;
reflection.Transparency = 0.5;
reflection.Size = 50;
reflection.Blur = 5;
reflection.Distance = 10;
// Save the workbook to see the effect
workbook.Save("ReflectionEffectFadeDirectionDemo.xlsx");
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
