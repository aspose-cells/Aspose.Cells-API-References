##TextBoxActiveXControl.SpecialEffect
TextBoxActiveXControl property. Gets and sets the special effect of the control
## TextBoxActiveXControl.SpecialEffect property
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
public class TextBoxActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an ActiveX TextBox control
var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 100, 100, 0, 0);
TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
// Set the SpecialEffect property
textBox.SpecialEffect = ControlSpecialEffectType.Bump;
// Save the workbook
workbook.Save("TextBoxActiveXControlSpecialEffectDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
