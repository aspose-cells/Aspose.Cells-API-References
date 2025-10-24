##CheckBoxActiveXControl.PicturePosition
CheckBoxActiveXControl property. Gets and set the location of the controls picture relative to its caption
## CheckBoxActiveXControl.PicturePosition property
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
public class CheckBoxActiveXControlPropertyPicturePositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CheckBox ActiveX control with all required parameters
var shape = worksheet.Shapes.AddActiveXControl(
ControlType.CheckBox,
10,  // left
10,  // top
150, // width
30,  // height
0,   // leftOffset
0    // topOffset
);
CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
// Configure the CheckBox properties
checkBox.Caption = "Sample CheckBox";
checkBox.PicturePosition = ControlPicturePositionType.Center;
checkBox.IsAutoSize = true;
// Save the workbook
workbook.Save("CheckBoxPicturePositionDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
