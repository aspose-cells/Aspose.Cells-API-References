##ToggleButtonActiveXControl.PicturePosition
ToggleButtonActiveXControl property. Gets and set the location of the controls picture relative to its caption
## ToggleButtonActiveXControl.PicturePosition property
Gets and set the location of the control's picture relative to its caption.
```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyPicturePositionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
var control = shape.ActiveXControl;
if (control is ToggleButtonActiveXControl toggleButton)
{
// Set PicturePosition property
toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;
// Set other properties to demonstrate functionality
toggleButton.Caption = "Toggle Button";
toggleButton.Picture = new byte[0]; // Empty picture for demo
}
// Save the workbook
workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
