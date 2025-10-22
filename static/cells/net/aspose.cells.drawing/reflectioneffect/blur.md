##ReflectionEffect.Blur
ReflectionEffect property. Gets and sets the blur radiusin unit of points
## ReflectionEffect.Blur property
Gets and sets the blur radius,in unit of points.
```csharp
public double Blur { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ReflectionEffectPropertyBlurDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Aspose.Cells.Drawing.Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
// Access reflection effect
Aspose.Cells.Drawing.ReflectionEffect reflection = rectangle.Reflection;
// Set reflection type and properties
reflection.Type = Aspose.Cells.Drawing.ReflectionEffectType.HalfReflectionTouching;
reflection.Blur = 0.5; // Demonstrate Blur property
reflection.Transparency = 0.5;
reflection.Size = 55;
reflection.Distance = 0;
// Save the workbook
workbook.Save("ReflectionEffectDemo.xlsx");
// Display blur value
Console.WriteLine("Reflection Blur: " + reflection.Blur);
}
}
}
```
### See Also
* class [ReflectionEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
