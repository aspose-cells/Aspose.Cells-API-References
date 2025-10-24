##ToggleButtonActiveXControl.SpecialEffect
ToggleButtonActiveXControl property. Gets and sets the special effect of the control
## ToggleButtonActiveXControl.SpecialEffect property
Gets and sets the special effect of the control.
```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;
// Set the SpecialEffect property
control.SpecialEffect = ControlSpecialEffectType.Bump;
// Save the workbook
workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
