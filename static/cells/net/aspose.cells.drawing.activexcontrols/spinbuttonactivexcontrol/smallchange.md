##SpinButtonActiveXControl.SmallChange
SpinButtonActiveXControl property. Gets and sets the amount by which the Position property changes
## SpinButtonActiveXControl.SmallChange property
Gets and sets the amount by which the Position property changes
```csharp
public int SmallChange { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpinButtonActiveXControlPropertySmallChangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(
Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
// Get the ActiveX control and set the SmallChange property
var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
spinButton.SmallChange = 5;
// Save the workbook
workbook.Save("SpinButtonSmallChangeDemo.xlsx");
}
}
}
```
### See Also
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
