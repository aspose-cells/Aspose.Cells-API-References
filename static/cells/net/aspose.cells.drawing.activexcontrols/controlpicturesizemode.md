##Enum ControlPictureSizeMode
Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode enum. Represents how to display the picture
## ControlPictureSizeMode enumeration
Represents how to display the picture.
```csharp
public enum ControlPictureSizeMode
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Clip | `0` | Crops any part of the picture that is larger than the control's boundaries. |
| Stretch | `1` | Stretches the picture to fill the control's area. This setting distorts the picture in either the horizontal or vertical direction. |
| Zoom | `3` | Enlarges the picture, but does not distort the picture in either the horizontal or vertical direction. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System.IO;
public class ControlPictureSizeModeDemo
{
public static void ControlPictureSizeModeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add an image to the worksheet
int pictureIndex = worksheet.Pictures.Add(1, 1, "ControlPictureSizeMode.png");
Picture picture = worksheet.Pictures[pictureIndex];
// Add an ImageActiveXControl to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 5, 5,5,100, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Set the picture data for the ImageActiveXControl
imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");
// Set the PictureSizeMode to Zoom
imageControl.PictureSizeMode = ControlPictureSizeMode.Zoom;
// Set other properties of the ImageActiveXControl
imageControl.IsAutoSize = true;
imageControl.BorderStyle = ControlBorderType.Single;
imageControl.BorderOleColor = 0x000000; // Black color
imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
imageControl.IsTiled = false;
// Save the workbook
workbook.Save("ControlPictureSizeModeExample.xlsx");
workbook.Save("ControlPictureSizeModeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
