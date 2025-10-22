##Class ImageActiveXControl
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl class. Represents the image control
## ImageActiveXControl class
Represents the image control.
```csharp
public class ImageActiveXControl : ActiveXControl
```
## Properties
| Name | Description |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Gets and sets the ole color of the background.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/) { get; set; } | Gets and sets the ole color of the background. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/) { get; set; } | Gets and set the type of border used by the control. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Gets and sets the binary data of the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Represents the font of the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Gets and sets the ole color of the foreground.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Gets and sets the height of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| override [IsAutoSize](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/) { get; set; } | Indicates whether the control will automatically resize to display its entire contents. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indicates whether the control can receive the focus and respond to user-generated events.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indicates whether data in the control is locked for editing.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [IsTiled](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/) { get; set; } | Indicates whether the picture is tiled across the background. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indicates whether the control is transparent.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indicates whether this control is visible.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Gets and sets the linked cell.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Gets and sets the list fill range.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Gets and sets a custom icon to display as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Gets and sets the type of icon displayed as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/) { get; set; } | Gets and sets the data of the picture. |
| [PictureAlignment](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/) { get; set; } | Gets and sets the alignment of the picture inside the Form or Image. |
| [PictureSizeMode](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/) { get; set; } | Gets and sets how to display the picture. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indicates whether to show a shadow.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/) { get; set; } | Gets and sets the special effect of the control. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Represents how to align the text used by the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/) { get; } | Gets the type of the ActiveX control. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Gets and sets the width of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Gets the [`Workbook`](../activexcontrolbase/workbook/) object.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
using System.IO;
namespace AsposeCellsExamples
{
public class ImageActiveXControlDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add an Image ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Set properties for the Image ActiveX control
imageControl.IsAutoSize = true;
imageControl.BorderOleColor = 0x000000; // Black border
imageControl.BorderStyle = ControlBorderType.Single;
imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
imageControl.IsTiled = false;
// Load an image from file and set it to the control
byte[] imageData = File.ReadAllBytes("ImageActiveXControlDemo.jpg");
imageControl.Picture = imageData;
// Save the workbook
workbook.Save("ImageActiveXControlDemo.xlsx");
workbook.Save("ImageActiveXControlDemo.pdf");
// Output the results
Console.WriteLine("Image ActiveX Control added with the following properties:");
Console.WriteLine($"IsAutoSize: {imageControl.IsAutoSize}");
Console.WriteLine($"BorderOleColor: {imageControl.BorderOleColor}");
Console.WriteLine($"BorderStyle: {imageControl.BorderStyle}");
Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
Console.WriteLine($"SpecialEffect: {imageControl.SpecialEffect}");
Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
Console.WriteLine($"IsTiled: {imageControl.IsTiled}");
}
}
}
```
### See Also
* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
