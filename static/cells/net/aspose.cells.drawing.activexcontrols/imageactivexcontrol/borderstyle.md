##ImageActiveXControl.BorderStyle
ImageActiveXControl property. Gets and set the type of border used by the control
## ImageActiveXControl.BorderStyle property
Gets and set the type of border used by the control.
```csharp
public ControlBorderType BorderStyle { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyBorderStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.Image,
5, 5, 100, 100, 200, 200);
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl =
(Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;
// Set border style and demonstrate its usage
imageControl.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
imageControl.BorderOleColor = 0x000000; // Black border
// Set sample image (ensure this file exists in your execution directory)
if (File.Exists("sample.png"))
{
imageControl.Picture = File.ReadAllBytes("sample.png");
}
workbook.Save("ImageActiveXControlBorderStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlBorderType](../../controlbordertype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
