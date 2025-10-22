##Enum ControlPictureAlignmentType
Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType enum. Represents the alignment of the picture inside the Form or Image
## ControlPictureAlignmentType enumeration
Represents the alignment of the picture inside the Form or Image.
```csharp
public enum ControlPictureAlignmentType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| TopLeft | `0` | The top left corner. |
| TopRight | `1` | The top right corner. |
| Center | `2` | The center. |
| BottomLeft | `3` | The bottom left corner. |
| BottomRight | `4` | The bottom right corner. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ActiveXControlsClassControlPictureAlignmentTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ImageActiveXControl with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.Image,
10,  // left
10,  // top
200, // width
200, // height
0,   // imageWidth
0    // imageHeight
);
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl =
(Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;
// Set image properties
imageControl.Picture = File.ReadAllBytes("sample.png");
imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Stretch;
// Save the workbook
workbook.Save("ImageControlDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
