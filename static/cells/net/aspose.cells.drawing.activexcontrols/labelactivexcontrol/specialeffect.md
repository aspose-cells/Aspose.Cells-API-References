##LabelActiveXControl.SpecialEffect
LabelActiveXControl property. Gets and sets the special effect of the control
## LabelActiveXControl.SpecialEffect property
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
public class LabelActiveXControlPropertySpecialEffectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a Label ActiveX Control with all required parameters
Shape shape = worksheet.Shapes.AddActiveXControl(
ControlType.Label,
1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
100, 50);       // heightInPx, widthInPx
LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;
// Set basic properties
labelControl.Caption = "Sample Label";
labelControl.IsWordWrapped = true;
// Demonstrate SpecialEffect property
labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);
// Change SpecialEffect and show the difference
labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);
// Save the workbook
workbook.Save("LabelActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
