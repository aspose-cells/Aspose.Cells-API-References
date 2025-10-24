##ReflectionEffect.Transparency
ReflectionEffect property. Gets and sets the degree of the starting reflection transparency as a value from 0.0 opaque through 1.0 clear
## ReflectionEffect.Transparency property
Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ReflectionEffectPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a rectangle shape to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 150);
// Get the reflection effect and set its properties
Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
reflection.Transparency = 0.5; // Demonstrate transparency property
reflection.Size = 55;
reflection.Blur = 0.5;
reflection.Distance = 0;
// Save the workbook
workbook.Save("ReflectionEffectDemo.xlsx");
// Verify the saved properties
Workbook loadedWorkbook = new Workbook("ReflectionEffectDemo.xlsx");
Aspose.Cells.Drawing.ReflectionEffect loadedReflection = loadedWorkbook.Worksheets[0].Shapes[0].Reflection;
Console.WriteLine("Reflection Type: " + loadedReflection.Type);
Console.WriteLine("Transparency: " + loadedReflection.Transparency);
Console.WriteLine("Size: " + loadedReflection.Size);
Console.WriteLine("Blur: " + loadedReflection.Blur);
Console.WriteLine("Distance: " + loadedReflection.Distance);
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
