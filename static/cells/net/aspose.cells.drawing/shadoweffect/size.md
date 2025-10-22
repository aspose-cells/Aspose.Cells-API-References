##ShadowEffect.Size
ShadowEffect property. Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow
## ShadowEffect.Size property
Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow.
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
public class ShadowEffectPropertySizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook book = new Workbook();
// Access first worksheet and add a shape
Worksheet sheet = book.Worksheets[0];
Shape shape = sheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Get the shadow effect and set properties including Size
ShadowEffect shadow = shape.ShadowEffect;
shadow.Angle = 150;
shadow.Blur = 30;
shadow.Size = 1.3; // Demonstrating Size property usage
shadow.Transparency = 0.4;
shadow.Distance = 80;
// Save the workbook
book.Save("ShadowEffectExample.xlsx");
Console.WriteLine("Shadow effect with Size property set to 1.3 has been applied.");
}
}
}
```
### See Also
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
