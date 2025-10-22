##ToggleButtonActiveXControl.Picture
ToggleButtonActiveXControl property. Gets and sets the data of the picture
## ToggleButtonActiveXControl.Picture property
Gets and sets the data of the picture.
```csharp
public byte[] Picture { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyPictureDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control and get its ActiveXControl property
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;
// Set picture for the toggle button
byte[] data = File.ReadAllBytes("image.png");
toggleButton.Picture = data;
// Save the workbook
workbook.Save("ToggleButtonWithPicture.xlsx");
}
}
}
```
### See Also
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
