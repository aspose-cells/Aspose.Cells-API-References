##ReflectionEffect.Size
ReflectionEffect property. Gets and sets the end position along the alpha gradient ramp of the end alpha valuein unit of percentage
## ReflectionEffect.Size property
Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage
```csharp
public double Size { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ReflectionEffectPropertySizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Set reflection properties including Size
ReflectionEffect reflection = shape.Reflection;
reflection.Type = ReflectionEffectType.HalfReflection4PtOffset;
reflection.Transparency = 0.5;
reflection.Size = 55.5;
reflection.Blur = 0.5;
reflection.Distance = 4;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the saved reflection properties
Workbook loadedWorkbook = new Workbook("output.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
ReflectionEffect loadedReflection = loadedShape.Reflection;
Console.WriteLine("Reflection Size: " + loadedReflection.Size);
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
