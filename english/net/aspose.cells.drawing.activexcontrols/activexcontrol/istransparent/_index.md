---
title: ActiveXControl.IsTransparent
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Indicates whether the control is transparent
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Indicates whether the control is transparent.

```csharp
public bool IsTransparent { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, control.IsTransparent);
private void Property_IsTransparent(ActiveXControl c)
        {
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)c;
            Assert.AreEqual(ControlType.ToggleButton, control.Type);
            Assert.AreEqual("ToggleButton1", control.Caption);
            Assert.AreEqual(ControlPicturePositionType.AboveCenter, control.PicturePosition);
            Assert.AreEqual(ControlSpecialEffectType.Sunken, control.SpecialEffect);
            Assert.AreEqual(null, control.Picture);
            Assert.AreEqual((char)0, control.Accelerator);
            Assert.AreEqual(CheckValueType.UnChecked, control.Value);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(66.755905511811, control.Width);
            //Assert.AreEqual(41.244094488189, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            //Assert.AreEqual(-2147483640, control.ForeOleColor);
            //Assert.AreEqual(-2147483635, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


