##ShadowEffect.Angle
ShadowEffect property. Gets and sets the lighting angle. Range from 0 to 359.9 degrees
## ShadowEffect.Angle property
Gets and sets the lighting angle. Range from 0 to 359.9 degrees.
```csharp
public double Angle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShadowEffectPropertyAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and set shadow effect angle
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
shape.ShadowEffect.Angle = 45;
// Verify and output the angle value
Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
