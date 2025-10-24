##SpinButtonActiveXControl.Orientation
SpinButtonActiveXControl property. Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally
## SpinButtonActiveXControl.Orientation property
Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally.
```csharp
public ControlScrollOrientation Orientation { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class SpinButtonActiveXControlPropertyOrientationDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a SpinButton ActiveX control
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
// Check and modify orientation
if (spinButton.Orientation == ControlScrollOrientation.Auto)
{
spinButton.Orientation = ControlScrollOrientation.Horizontal;
}
// Save the workbook
workbook.Save("SpinButtonOrientationDemo.xlsx");
}
}
}
```
### See Also
* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
