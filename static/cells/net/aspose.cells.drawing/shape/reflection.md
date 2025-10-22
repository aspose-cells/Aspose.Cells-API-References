##Shape.Reflection
Shape property. Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape
## Shape.Reflection property
Represents a [`ReflectionEffect`](../../reflectioneffect/) object that specifies reflection effect for the chart element or shape.
```csharp
public ReflectionEffect Reflection { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyReflectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
// Set reflection properties
ReflectionEffect reflection = shape.Reflection;
reflection.Blur = 5;
reflection.Distance = 10;
reflection.Direction = 90;
reflection.FadeDirection = 90;
reflection.Size = 50;
reflection.Transparency = 0.5;
reflection.Type = ReflectionEffectType.None;
// Save the workbook
workbook.Save("ShapeReflectionDemo.xlsx");
}
}
}
```
### See Also
* class [ReflectionEffect](../../reflectioneffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
