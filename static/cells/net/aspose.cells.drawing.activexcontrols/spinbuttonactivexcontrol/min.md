##SpinButtonActiveXControl.Min
SpinButtonActiveXControl property. Gets and sets the minimum acceptable value
## SpinButtonActiveXControl.Min property
Gets and sets the minimum acceptable value.
```csharp
public int Min { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpinButtonActiveXControlPropertyMinDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton =
(Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
// Set the Min property of the SpinButton
spinButton.Min = 0;
// Set other properties to demonstrate functionality
spinButton.Max = 100;
spinButton.Position = 50;
// Save the workbook
workbook.Save("SpinButtonMinDemo.xlsx");
}
}
}
```
### See Also
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
