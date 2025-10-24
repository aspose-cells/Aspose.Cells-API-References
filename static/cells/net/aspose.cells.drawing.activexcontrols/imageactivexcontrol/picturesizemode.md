##ImageActiveXControl.PictureSizeMode
ImageActiveXControl property. Gets and sets how to display the picture
## ImageActiveXControl.PictureSizeMode property
Gets and sets how to display the picture.
```csharp
public ControlPictureSizeMode PictureSizeMode { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyPictureSizeModeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add an Image ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 1, 1, 200, 200, 0, 0);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Set PictureSizeMode and other properties
imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
// Load a sample image (replace with your own image path)
string imagePath = "sample.jpg";
if (File.Exists(imagePath))
{
byte[] imageData = File.ReadAllBytes(imagePath);
imageControl.Picture = imageData;
}
// Save the workbook
workbook.Save("ImageActiveXControlDemo.xlsx");
// Output the PictureSizeMode value
Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
}
}
}
```
### See Also
* enum [ControlPictureSizeMode](../../controlpicturesizemode/)
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
