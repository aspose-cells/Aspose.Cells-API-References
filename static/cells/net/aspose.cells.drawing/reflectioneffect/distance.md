##ReflectionEffect.Distance
ReflectionEffect property. Gets and sets how far to distance the shadowin unit of points
## ReflectionEffect.Distance property
Gets and sets how far to distance the shadow,in unit of points.
```csharp
public double Distance { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ReflectionEffectPropertyDistanceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to test reflection - fixed parameters to match method signature
Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Set reflection properties
ReflectionEffect reflection = shape.Reflection;
reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
reflection.Transparency = 0.5;
reflection.Size = 55.5;
reflection.Blur = 0.5;
reflection.Distance = 4; // Demonstrating Distance property
// Save and reload to verify persistence
string outputPath = "ReflectionEffectDemo.xlsx";
workbook.Save(outputPath);
// Reload to verify
Workbook loadedWorkbook = new Workbook(outputPath);
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
ReflectionEffect loadedReflection = loadedShape.Reflection;
Console.WriteLine("Original Distance: " + reflection.Distance);
Console.WriteLine("Loaded Distance: " + loadedReflection.Distance);
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
