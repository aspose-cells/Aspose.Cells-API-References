##ImageActiveXControl.IsAutoSize
ImageActiveXControl property. Indicates whether the control will automatically resize to display its entire contents
## ImageActiveXControl.IsAutoSize property
Indicates whether the control will automatically resize to display its entire contents.
```csharp
public override bool IsAutoSize { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageActiveXControlPropertyIsAutoSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ImageActiveXControl to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.Image,
5,  // left
5,  // top
100, // width
100, // height
0,   // imageWidth (0 for default)
0    // imageHeight (0 for default)
);
Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl imageControl =
(Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl)shape.ActiveXControl;
// Set the picture data (ensure the image file exists)
imageControl.Picture = File.ReadAllBytes("ControlPictureSizeMode.png");
// Demonstrate IsAutoSize property
imageControl.IsAutoSize = true; // Control will automatically resize to fit the image
imageControl.PictureSizeMode = Aspose.Cells.Drawing.ActiveXControls.ControlPictureSizeMode.Zoom;
// Save the workbook
workbook.Save("ImageActiveXControlIsAutoSizeDemo.xlsx");
}
}
}
```
### See Also
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
