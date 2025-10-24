##SpinButtonActiveXControl.Max
SpinButtonActiveXControl property. Gets and sets the maximum acceptable value
## SpinButtonActiveXControl.Max property
Gets and sets the maximum acceptable value.
```csharp
public int Max { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpinButtonActiveXControlPropertyMaxDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
// Get the ActiveX control and set its Max property
var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
spinButton.Max = 100;
// Save the workbook
workbook.Save("SpinButtonMaxDemo.xlsx");
}
}
}
```
### See Also
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
