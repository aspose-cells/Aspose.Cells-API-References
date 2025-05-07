---
title: ActiveXControlBase.MouseIcon
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets a custom icon to display as the mouse pointer for the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/
---
## ActiveXControlBase.MouseIcon property

Gets and sets a custom icon to display as the mouse pointer for the control.

```csharp
public byte[] MouseIcon { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(null, control.MouseIcon);
private void Property_MouseIcon(ActiveXControl c)
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

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


