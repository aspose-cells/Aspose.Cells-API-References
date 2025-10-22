##LabelActiveXControl.Picture
LabelActiveXControl property. Gets and sets the data of the picture
## LabelActiveXControl.Picture property
Gets and sets the data of the picture.
```csharp
public byte[] Picture { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a Label ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;
// Set basic properties
labelControl.Caption = "Sample Label";
labelControl.PicturePosition = ControlPicturePositionType.LeftTop;
// Load an image for the Picture property
string imagePath = "sample.jpg"; // Replace with actual image path
if (File.Exists(imagePath))
{
labelControl.Picture = File.ReadAllBytes(imagePath);
Console.WriteLine("Picture set successfully");
}
else
{
Console.WriteLine("Image file not found, using null picture");
labelControl.Picture = null;
}
// Save the workbook
workbook.Save("LabelActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
