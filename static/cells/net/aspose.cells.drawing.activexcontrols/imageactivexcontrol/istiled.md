##ImageActiveXControl.IsTiled
ImageActiveXControl property. Indicates whether the picture is tiled across the background
## ImageActiveXControl.IsTiled property
Indicates whether the picture is tiled across the background.
```csharp
public bool IsTiled { get; set; }
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
public class ImageActiveXControlPropertyIsTiledDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add an Image ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;
// Set IsTiled property and other properties
imageControl.IsTiled = true;
imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
// Load an image from file (replace with your own image path)
byte[] imageData = File.ReadAllBytes("demo.jpg");
imageControl.Picture = imageData;
// Save the workbook
workbook.Save("ImageActiveXControlIsTiledDemo.xlsx");
Console.WriteLine($"IsTiled property set to: {imageControl.IsTiled}");
}
}
}
```
### See Also
* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
