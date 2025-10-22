##Class CommandButtonActiveXControl
Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl class. Represents a command button
## CommandButtonActiveXControl class
Represents a command button.
```csharp
public class CommandButtonActiveXControl : ActiveXControl
```
## Properties
| Name | Description |
| --- | --- |
| [Accelerator](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/) { get; set; } | Gets and sets the accelerator key for the control. |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Gets and sets the ole color of the background.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Caption](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/) { get; set; } | Gets and set the descriptive text that appears on a control. |
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
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/) { get; set; } | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Gets and sets the linked cell.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Gets and sets the list fill range.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Gets and sets a custom icon to display as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Gets and sets the type of icon displayed as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/) { get; set; } | Gets and sets the data of the picture. |
| [PicturePosition](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/) { get; set; } | Gets and set the location of the control's picture relative to its caption. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indicates whether to show a shadow.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TakeFocusOnClick](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/) { get; set; } | Indicates whether the control takes the focus when clicked. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Represents how to align the text used by the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/) { get; } | Gets the type of the ActiveX control. |
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
public class CommandButtonActiveXControlDemo
{
public static void CommandButtonActiveXControlExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a CommandButton ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;
// Set properties of the CommandButton ActiveX control
commandButton.Caption = "Click Me";
commandButton.PicturePosition = ControlPicturePositionType.Center;
commandButton.Accelerator = 'C';
commandButton.TakeFocusOnClick = true;
commandButton.IsWordWrapped = true;
commandButton.IsEnabled = true;
commandButton.IsLocked = false;
commandButton.IsTransparent = false;
commandButton.IsAutoSize = false;
commandButton.IMEMode = InputMethodEditorMode.NoControl;
commandButton.TextAlign = TextAlignmentType.Center;
commandButton.Width = 150;
commandButton.Height = 50;
commandButton.MousePointer = ControlMousePointerType.Default;
commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
commandButton.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
commandButton.IsVisible = true;
commandButton.Shadow = true;
commandButton.LinkedCell = "A1";
commandButton.ListFillRange = "A2:A10";
// Save the workbook
workbook.Save("CommandButtonActiveXControlExample.xlsx");
workbook.Save("CommandButtonActiveXControlExample.pdf");
}
}
}
```
### See Also
* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
