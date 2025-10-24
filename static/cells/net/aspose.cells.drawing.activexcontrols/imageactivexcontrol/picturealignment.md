##ImageActiveXControl.PictureAlignment
ImageActiveXControl property. Gets and sets the alignment of the picture inside the Form or Image
## ImageActiveXControl.PictureAlignment property
Gets and sets the alignment of the picture inside the Form or Image.
```csharp
public ControlPictureAlignmentType PictureAlignment { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyPictureAlignmentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.Image, 5, 0, 1, 1, 100, 100);
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl = (Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;
// Set PictureAlignment property
imageControl.PictureAlignment = Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType.Center;
// Load sample image (replace with actual image path)
string imagePath = "sample.jpg";
if (File.Exists(imagePath))
{
byte[] imageData = File.ReadAllBytes(imagePath);
imageControl.Picture = imageData;
}
workbook.Save("ImageActiveXControlDemo.xlsx");
Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
}
}
}
```
### See Also
* enum [ControlPictureAlignmentType](../../controlpicturealignmenttype/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
