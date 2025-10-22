##SpinButtonActiveXControl.Type
SpinButtonActiveXControl property. Gets the type of the ActiveX control
## SpinButtonActiveXControl.Type property
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
public class SpinButtonActiveXControlPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control (parameters: left, top, width, height)
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
// Check the control type using Type property
if (spinButton.Type == ControlType.SpinButton)
{
// Set some properties specific to SpinButton
spinButton.Min = 0;
spinButton.Max = 100;
spinButton.Position = 50;
spinButton.SmallChange = 1;
}
// Save the workbook
workbook.Save("SpinButtonActiveXControlDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
