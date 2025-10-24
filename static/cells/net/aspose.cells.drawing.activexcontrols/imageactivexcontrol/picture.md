##ImageActiveXControl.Picture
ImageActiveXControl property. Gets and sets the data of the picture
## ImageActiveXControl.Picture property
Gets and sets the data of the picture.
```csharp
public byte[] Picture { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an Image ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 100, 100, 100, 100);
ImageActiveXControl imgControl = (ImageActiveXControl)shape.ActiveXControl;
// Set properties
imgControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
imgControl.PictureAlignment = ControlPictureAlignmentType.TopLeft;
imgControl.IsTiled = false;
// Set the Picture property (using a sample image byte array)
byte[] imageData = new byte[] { 0x00, 0x01, 0x02 }; // Sample image data
imgControl.Picture = imageData;
// Verify the Picture property was set
Console.WriteLine("Picture data length: " + imgControl.Picture.Length);
// Save the workbook
workbook.Save("ImageActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
