##Enum ControlScrollOrientation
Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation enum. Represents type of scroll orientation
## ControlScrollOrientation enumeration
Represents type of scroll orientation
```csharp
public enum ControlScrollOrientation
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Auto | `3` | Control is rendered horizontally when the control's width is greater than its height. Control is rendered vertically otherwise. |
| Vertical | `0` | Control is rendered vertically. |
| Horizontal | `1` | Control is rendered horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class ControlScrollOrientationDemo
{
public static void ControlScrollOrientationExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
// Add a ScrollBarActiveXControl to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;
// Set properties for the ScrollBarActiveXControl
activeXControl.LargeChange = 5;
activeXControl.Min = 0;
activeXControl.Max = 100;
activeXControl.Position = 30;
activeXControl.SmallChange = 5;
// Demonstrate setting the orientation using ControlScrollOrientation enum
if (activeXControl.Orientation == ControlScrollOrientation.Auto)
{
activeXControl.Orientation = ControlScrollOrientation.Horizontal;
}
// Save the workbook
workbook.Save("ControlScrollOrientationExample.xlsx");
workbook.Save("ControlScrollOrientationExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
