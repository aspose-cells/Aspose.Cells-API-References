##SpinButtonActiveXControl.Position
SpinButtonActiveXControl property. Gets and sets the value
## SpinButtonActiveXControl.Position property
Gets and sets the value.
```csharp
public int Position { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpinButtonActiveXControlPropertyPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
1, 0, 1, 0, 100, 30);
// Get the ActiveX control and set Position property
var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
spinButton.Position = 30;
// Save the workbook
workbook.Save("SpinButtonPositionDemo.xlsx");
}
}
}
```
### See Also
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
