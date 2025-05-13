---
title: Class ActiveXControl
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ActiveXControls.ActiveXControl class. Represents the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Represents the ActiveX control.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Properties

| Name | Description |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Gets and sets the ole color of the background.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Gets and sets the binary data of the control. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Represents the font of the control. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Gets and sets the ole color of the foreground.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Gets and sets the height of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indicates whether the control will automatically resize to display its entire contents. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indicates whether the control can receive the focus and respond to user-generated events. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indicates whether data in the control is locked for editing. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indicates whether the control is transparent. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indicates whether this control is visible.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Gets and sets the linked cell.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Gets and sets the list fill range.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Gets and sets a custom icon to display as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Gets and sets the type of icon displayed as the mouse pointer for the control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indicates whether to show a shadow.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Represents how to align the text used by the control. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Gets the type of the ActiveX control.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Gets and sets the width of the control in unit of points.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Gets the [`Workbook`](../activexcontrolbase/workbook/) object.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |

### Examples

```csharp
// Called: private void CheckRadioButtonActiveXControl(ActiveXControl c)
private void ActiveXControls_Type_ActiveXControl(ActiveXControl c)
        {
            RadioButtonActiveXControl control = (RadioButtonActiveXControl)c;
            Assert.AreEqual(ControlType.RadioButton, control.Type);
            Assert.AreEqual("Sheet1", control.GroupName);
            Assert.AreEqual(ControlCaptionAlignmentType.Left, control.Alignment);
            Assert.AreEqual(true, control.IsWordWrapped);
            Assert.AreEqual("OptionButton1", control.Caption);
            Assert.AreEqual(ControlPicturePositionType.AboveCenter, control.PicturePosition);
            Assert.AreEqual(ControlSpecialEffectType.Sunken, control.SpecialEffect);
            Assert.AreEqual(null, control.Picture);
            Assert.AreEqual((char)0, control.Accelerator);
            //Assert.AreEqual(CheckValueType.UnChecked, control.Value);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(81.0141732283465, control.Width);
            //Assert.AreEqual(42.7464566929134, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            //Assert.AreEqual(-2147483640, control.ForeOleColor);
            //Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


