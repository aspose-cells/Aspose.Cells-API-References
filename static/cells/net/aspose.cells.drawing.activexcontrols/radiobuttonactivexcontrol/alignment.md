##RadioButtonActiveXControl.Alignment
RadioButtonActiveXControl property. Gets and set the position of the Caption relative to the control
## RadioButtonActiveXControl.Alignment property
Gets and set the position of the Caption relative to the control.
```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class RadioButtonActiveXControlPropertyAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create a new shape collection and add ActiveX control
ShapeCollection shapes = worksheet.Shapes;
Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
// Set the Alignment property
radioButton.Alignment = ControlCaptionAlignmentType.Left;
// Save the workbook
workbook.Save("RadioButtonAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
