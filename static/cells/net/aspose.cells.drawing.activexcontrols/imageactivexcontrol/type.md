##ImageActiveXControl.Type
ImageActiveXControl property. Gets the type of the ActiveX control
## ImageActiveXControl.Type property
Gets the type of the ActiveX control.
```csharp
public override ControlType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add an Image ActiveX Control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 1, 1, 200, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Demonstrate Type property usage
Console.WriteLine("Control Type: " + imageControl.Type);
// Set some properties
imageControl.IsAutoSize = false;
imageControl.BorderStyle = ControlBorderType.Single;
imageControl.PictureSizeMode = ControlPictureSizeMode.Clip;
// Save the workbook
workbook.Save("ImageActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
