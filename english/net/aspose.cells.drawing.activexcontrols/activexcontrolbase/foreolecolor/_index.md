---
title: ActiveXControlBase.ForeOleColor
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the ole color of the foreground
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/
---
## ActiveXControlBase.ForeOleColor property

Gets and sets the ole color of the foreground.

```csharp
public virtual int ForeOleColor { get; set; }
```

### Remarks

Not applies to Image control.

### Examples

```csharp
// Called: Assert.AreEqual(-2147483630, control.ForeOleColor);
private void Property_ForeOleColor(ActiveXControl c)
        {
            ImageActiveXControl control = (ImageActiveXControl)c;
            Assert.AreEqual(ControlType.Image, control.Type);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(-2147483642, control.BorderOleColor);
            Assert.AreEqual(ControlBorderType.Single, control.BorderStyle);
            Assert.AreEqual(ControlPictureSizeMode.Clip, control.PictureSizeMode);
            Assert.AreEqual(ControlSpecialEffectType.Flat, control.SpecialEffect);
            Assert.AreEqual(null, control.Picture);
            Assert.AreEqual(ControlPictureAlignmentType.Center, control.PictureAlignment);
            Assert.AreEqual(false, control.IsTiled);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("MS Sans Serif", control.Font.Name);
            //Assert.AreEqual(92.2393700787402, control.Width);
            //Assert.AreEqual(43.5118110236221, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


