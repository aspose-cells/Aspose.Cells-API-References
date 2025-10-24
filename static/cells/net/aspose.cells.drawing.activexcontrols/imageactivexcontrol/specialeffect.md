##ImageActiveXControl.SpecialEffect
ImageActiveXControl property. Gets and sets the special effect of the control
## ImageActiveXControl.SpecialEffect property
Gets and sets the special effect of the control.
```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Demonstrate SpecialEffect property
imageControl.SpecialEffect = ControlSpecialEffectType.Raised;
// Set other required properties
imageControl.BorderStyle = ControlBorderType.Single;
byte[] imageData = File.ReadAllBytes("demo.jpg");
imageControl.Picture = imageData;
workbook.Save("ImageActiveXControlSpecialEffectDemo.xlsx");
Console.WriteLine($"SpecialEffect set to: {imageControl.SpecialEffect}");
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
