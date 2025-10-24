##ActiveXControlBase.Type
ActiveXControlBase property. Gets the type of the ActiveX control
## ActiveXControlBase.Type property
Gets the type of the ActiveX control.
```csharp
public abstract ControlType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ActiveXControlBasePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a Label ActiveX control with correct parameters
Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
labelControl.Caption = "Label_ActiveX";
// Demonstrate Type property usage
if (labelShape.ActiveXControl.Type == ControlType.Label)
{
Console.WriteLine("The control is a Label type");
labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
}
// Save and verify
workbook.Save("output.xlsx");
Console.WriteLine("Label caption changed to: " + labelControl.Caption);
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
