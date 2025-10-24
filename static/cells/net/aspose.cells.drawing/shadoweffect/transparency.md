##ShadowEffect.Transparency
ShadowEffect property. Gets and sets the degree of transparency of the shadow. Range from 0.0 opaque to 1.0 clear
## ShadowEffect.Transparency property
Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear).
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
public class ShadowEffectPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate shadow effect
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Get shadow effect and set properties including Transparency
ShadowEffect shadow = shape.ShadowEffect;
shadow.Angle = 150;
shadow.Blur = 30;
shadow.Size = 1.3;
shadow.Transparency = 0.4; // Setting transparency to 40%
shadow.Distance = 80;
// Save the workbook
workbook.Save("ShadowEffectDemo.xlsx");
Console.WriteLine("Workbook saved with shadow effect transparency set to 0.4");
}
}
}
```
### See Also
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
