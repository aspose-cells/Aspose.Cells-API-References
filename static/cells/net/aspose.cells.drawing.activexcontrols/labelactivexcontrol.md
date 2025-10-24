##Class LabelActiveXControl
Aspose.Cells.Drawing.ActiveXControls.LabelActiveXControl class. Represents the label ActiveX control
## LabelActiveXControl class
Represents the label ActiveX control.
```csharp
public class LabelActiveXControl : ActiveXControl
```
## Properties
| Name | Description |
| --- | --- |
| [Accelerator](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/accelerator/) { get; set; } | Gets and sets the accelerator key for the control. |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Gets and sets the ole color of the background.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderolecolor/) { get; set; } | Gets and sets the ole color of the background. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/borderstyle/) { get; set; } | Gets and set the type of border used by the control. |
| [Caption](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/) { get; set; } | Gets and set the descriptive text that appears on a control. |
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
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/iswordwrapped/) { get; set; } | Indicates whether the contents of the control automatically wrap at the end of a line. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Gets and sets the linked cell.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Gets and sets the list fill range.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Gets and sets a custom icon to display as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Gets and sets the type of icon displayed as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/) { get; set; } | Gets and sets the data of the picture. |
| [PicturePosition](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/) { get; set; } | Gets and set the location of the control's picture relative to its caption. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indicates whether to show a shadow.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/) { get; set; } | Gets and sets the special effect of the control. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Represents how to align the text used by the control.(Inherited from [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/labelactivexcontrol/type/) { get; } | Gets the type of the ActiveX control. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Gets and sets the width of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Gets the [`Workbook`](../activexcontrolbase/workbook/) object.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
namespace AsposeCellsExamples
{
public class LabelActiveXControlDemo
{
public static void RunDemo()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add a Label ActiveX control to the worksheet
var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;
// Set properties for the Label
label.Caption = "Hello, Aspose!";
label.PicturePosition = ControlPicturePositionType.Center;
label.BorderOleColor = 0x000000; // Black color
label.BorderStyle = ControlBorderType.Single;
label.SpecialEffect = ControlSpecialEffectType.Flat;
label.Accelerator = 'H';
label.IsWordWrapped = true;
label.IsEnabled = true;
label.IsLocked = false;
label.IsTransparent = false;
label.IsAutoSize = true;
label.IMEMode = InputMethodEditorMode.NoControl;
label.TextAlign = TextAlignmentType.Center;
label.ForeOleColor = 0x000000; // Black color
label.BackOleColor = 0xFFFFFF; // White color
label.IsVisible = true;
label.Shadow = false;
// Save the workbook
workbook.Save("LabelActiveXControlDemo.xlsx");
// Output the results
Console.WriteLine("Label Caption: " + label.Caption);
Console.WriteLine("Label Picture Position: " + label.PicturePosition);
Console.WriteLine("Label Border Color: " + label.BorderOleColor);
Console.WriteLine("Label Border Style: " + label.BorderStyle);
Console.WriteLine("Label Special Effect: " + label.SpecialEffect);
Console.WriteLine("Label Accelerator: " + label.Accelerator);
Console.WriteLine("Label Is Word Wrapped: " + label.IsWordWrapped);
Console.WriteLine("Label Is Enabled: " + label.IsEnabled);
Console.WriteLine("Label Is Locked: " + label.IsLocked);
Console.WriteLine("Label Is Transparent: " + label.IsTransparent);
Console.WriteLine("Label Is Auto Size: " + label.IsAutoSize);
Console.WriteLine("Label IME Mode: " + label.IMEMode);
Console.WriteLine("Label Text Align: " + label.TextAlign);
Console.WriteLine("Label Fore Color: " + label.ForeOleColor);
Console.WriteLine("Label Back Color: " + label.BackOleColor);
Console.WriteLine("Label Is Visible: " + label.IsVisible);
Console.WriteLine("Label Shadow: " + label.Shadow);
}
}
}
```
### See Also
* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
