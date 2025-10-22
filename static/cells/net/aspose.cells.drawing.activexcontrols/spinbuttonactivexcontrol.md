##Class SpinButtonActiveXControl
Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl class. Represents the SpinButton control
## SpinButtonActiveXControl class
Represents the SpinButton control.
```csharp
public class SpinButtonActiveXControl : ActiveXControl
```
## Properties
| Name | Description |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Gets and sets the ole color of the background.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Gets and sets the binary data of the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Represents the font of the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Gets and sets the ole color of the foreground.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Gets and sets the height of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indicates whether the control will automatically resize to display its entire contents.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indicates whether the control can receive the focus and respond to user-generated events.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indicates whether data in the control is locked for editing.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indicates whether the control is transparent.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indicates whether this control is visible.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Gets and sets the linked cell.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Gets and sets the list fill range.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Max](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/) { get; set; } | Gets and sets the maximum acceptable value. |
| [Min](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/) { get; set; } | Gets and sets the minimum acceptable value. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Gets and sets a custom icon to display as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Gets and sets the type of icon displayed as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Orientation](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/) { get; set; } | Gets and sets whether the SpinButton or ScrollBar is oriented vertically or horizontally. |
| [Position](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/) { get; set; } | Gets and sets the value. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indicates whether to show a shadow.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SmallChange](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/) { get; set; } | Gets and sets the amount by which the Position property changes |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Represents how to align the text used by the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/) { get; } | Gets the type of the ActiveX control. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Gets and sets the width of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Gets the [`Workbook`](../activexcontrolbase/workbook/) object.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class SpinButtonActiveXControlDemo
{
public static void SpinButtonActiveXControlExample()
{
// Initialize a new workbook.
Workbook workbook = new Workbook();
// Add a SpinButtonActiveXControl.
Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.SpinButton, 1, 0, 1, 0, 100, 50);
SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.ActiveXControl;
// Setting properties
activeXControl.Min = 0;
activeXControl.Max = 100;
activeXControl.Position = 30;
activeXControl.SmallChange = 5;
if (activeXControl.Orientation == ControlScrollOrientation.Auto)
{
activeXControl.Orientation = ControlScrollOrientation.Horizontal;
}
activeXControl.IsEnabled = true;
activeXControl.IsLocked = false;
activeXControl.IsTransparent = false;
activeXControl.IsAutoSize = true;
activeXControl.IMEMode = InputMethodEditorMode.On;
activeXControl.TextAlign = TextAlignmentType.Center;
activeXControl.Width = 150;
activeXControl.Height = 30;
activeXControl.MousePointer = ControlMousePointerType.Default;
activeXControl.ForeOleColor = 0x000000; // Black color
activeXControl.BackOleColor = 0xFFFFFF; // White color
activeXControl.IsVisible = true;
activeXControl.Shadow = false;
activeXControl.LinkedCell = "A1";
activeXControl.ListFillRange = "A2:A10";
// Save the workbook
workbook.Save("SpinButtonActiveXControlExample.xlsx");
return;
}
}
}
```
### See Also
* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
