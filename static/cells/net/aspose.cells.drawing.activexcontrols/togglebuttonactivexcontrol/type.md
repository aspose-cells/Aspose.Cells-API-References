##ToggleButtonActiveXControl.Type
ToggleButtonActiveXControl property. Gets the type of the ActiveX control
## ToggleButtonActiveXControl.Type property
Gets the type of the ActiveX control.
```csharp
public override ControlType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class ToggleButtonActiveXControlPropertyTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a ToggleButton ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;
// Demonstrate Type property usage
ControlType type = toggleButton.Type;
Console.WriteLine("Control Type: " + type.ToString());
// Set some properties
toggleButton.Caption = "Click Me";
toggleButton.Value = CheckValueType.Checked;
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
