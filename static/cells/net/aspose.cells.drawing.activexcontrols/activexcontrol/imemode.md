##ActiveXControl.IMEMode
ActiveXControl property. Gets and sets the default runtime mode of the Input Method Editor for the control as it receives focus
## ActiveXControl.IMEMode property
Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.
```csharp
public InputMethodEditorMode IMEMode { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlPropertyIMEModeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control with proper coordinates
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.ToggleButton,
1, 1,  // Upper-left row/column
1, 1,  // Upper-left row/column offsets
100, 50);  // Width and height
ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;
// Set properties including IMEMode
toggleButton.Caption = "ToggleButton1";
toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
toggleButton.IMEMode = InputMethodEditorMode.NoControl;
// Verify and output the IMEMode property
Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);
// Save the workbook
workbook.Save("ActiveXControlIMEModeDemo.xlsx");
}
}
}
```
### See Also
* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
