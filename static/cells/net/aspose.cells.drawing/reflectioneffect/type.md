##ReflectionEffect.Type
ReflectionEffect property. Gets and sets the preset reflection effect
## ReflectionEffect.Type property
Gets and sets the preset reflection effect.
```csharp
public ReflectionEffectType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ReflectionEffectPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
// Get reflection effect
ReflectionEffect reflection = shape.Reflection;
// Demonstrate Type property
Console.WriteLine("Initial reflection type: " + reflection.Type);
// Change reflection type
reflection.Type = ReflectionEffectType.HalfReflectionTouching;
Console.WriteLine("Updated reflection type: " + reflection.Type);
// Set other reflection properties
reflection.Transparency = 0.5;
reflection.Size = 55;
reflection.Blur = 0.5;
reflection.Distance = 0;
// Save the workbook
workbook.Save("ReflectionEffectDemo.xlsx");
Console.WriteLine("Demo completed successfully.");
}
}
}
```
### See Also
* enum [ReflectionEffectType](../../reflectioneffecttype/)
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
