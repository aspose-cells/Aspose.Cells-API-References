##Class ReflectionEffect
Aspose.Cells.Drawing.ReflectionEffect class. This class specifies a reflection effect
## ReflectionEffect class
This class specifies a reflection effect.
```csharp
public class ReflectionEffect
```
## Properties
| Name | Description |
| --- | --- |
| [Blur](../../aspose.cells.drawing/reflectioneffect/blur/) { get; set; } | Gets and sets the blur radius,in unit of points. |
| [Direction](../../aspose.cells.drawing/reflectioneffect/direction/) { get; set; } | Gets and sets the direction of the alpha gradient ramp relative to the shape itself. |
| [Distance](../../aspose.cells.drawing/reflectioneffect/distance/) { get; set; } | Gets and sets how far to distance the shadow,in unit of points. |
| [FadeDirection](../../aspose.cells.drawing/reflectioneffect/fadedirection/) { get; set; } | Gets and sets the direction to offset the reflection. |
| [RotWithShape](../../aspose.cells.drawing/reflectioneffect/rotwithshape/) { get; set; } | Gets and sets if the reflection should rotate with the shape. |
| [Size](../../aspose.cells.drawing/reflectioneffect/size/) { get; set; } | Gets and sets the end position (along the alpha gradient ramp) of the end alpha value,in unit of percentage |
| [Transparency](../../aspose.cells.drawing/reflectioneffect/transparency/) { get; set; } | Gets and sets the degree of the starting reflection transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [Type](../../aspose.cells.drawing/reflectioneffect/type/) { get; set; } | Gets and sets the preset reflection effect. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassReflectionEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Set reflection effect properties
ReflectionEffect reflection = shape.Reflection;
reflection.Size = 90;
reflection.Blur = 30;
reflection.Transparency = 0.5;
reflection.Distance = 10;
// Display reflection properties
Console.WriteLine("Reflection Size: " + reflection.Size);
Console.WriteLine("Reflection Blur: " + reflection.Blur);
Console.WriteLine("Reflection Transparency: " + reflection.Transparency);
Console.WriteLine("Reflection Distance: " + reflection.Distance);
// Save the workbook
workbook.Save("ReflectionEffectDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
