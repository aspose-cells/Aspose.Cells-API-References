##LabelActiveXControl.PicturePosition
LabelActiveXControl property. Gets and set the location of the controls picture relative to its caption
## LabelActiveXControl.PicturePosition property
Gets and set the location of the control's picture relative to its caption.
```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class LabelActiveXControlPropertyPicturePositionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
label.Caption = "Demo Label";
label.PicturePosition = ControlPicturePositionType.AboveLeft;
Console.WriteLine("Label Picture Position: " + label.PicturePosition);
workbook.Save("LabelActiveXControlPicturePositionDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
