##ShadowEffect.Blur
ShadowEffect property. Gets and sets the blur of the shadow. Range from 0 to 100 points
## ShadowEffect.Blur property
Gets and sets the blur of the shadow. Range from 0 to 100 points.
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
public class ShadowEffectPropertyBlurDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Get shadow effect
ShadowEffect shadow = shape.ShadowEffect;
// Set shadow properties including Blur
shadow.Angle = 150;
shadow.Blur = 30;
shadow.Size = 1.3;
shadow.Transparency = 0.4;
shadow.Distance = 80;
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("Shadow effect with blur applied successfully.");
}
}
}
```
### See Also
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
