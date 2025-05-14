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
private void ActiveXControl_Property_IsTransparent(ActiveXControl c)
        {
            LabelActiveXControl control = (LabelActiveXControl)c;
            Assert.AreEqual(ControlType.Label, control.Type);
            Assert.AreEqual("Label1aaaa", control.Caption);
            Assert.AreEqual(ControlPicturePositionType.LeftTop, control.PicturePosition);
            Assert.AreEqual(-2147483642, control.BorderOleColor);
            Assert.AreEqual(ControlBorderType.None, control.BorderStyle);
            Assert.AreEqual(ControlSpecialEffectType.Flat, control.SpecialEffect);
            Assert.AreEqual(null, control.Picture);
            Assert.AreEqual((char)0, control.Accelerator);
            Assert.AreEqual(true, control.IsWordWrapped);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(73.5023622047244, control.Width);
            //Assert.AreEqual(33.7606299212598, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Cross, control.MousePointer);
            Assert.AreEqual(-2147483640, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


