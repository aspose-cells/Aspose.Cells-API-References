##ToggleButtonActiveXControl.Caption
ToggleButtonActiveXControl property. Gets and set the descriptive text that appears on a control
## ToggleButtonActiveXControl.Caption property
Gets and set the descriptive text that appears on a control.
```csharp
public string Caption { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyCaptionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.ToggleButton, 2, 0, 2, 0, 100, 30);
ToggleButtonActiveXControl toggleButtonControl = (ToggleButtonActiveXControl)shape.ActiveXControl;
toggleButtonControl.Caption = "ExampleButton";
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
