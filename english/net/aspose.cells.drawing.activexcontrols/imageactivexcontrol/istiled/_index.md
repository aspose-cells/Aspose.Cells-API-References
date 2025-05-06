---
title: ImageActiveXControl.IsTiled
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Indicates whether the picture is tiled across the background
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/
---
## ImageActiveXControl.IsTiled property

Indicates whether the picture is tiled across the background.

```csharp
public bool IsTiled { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, control.IsTiled);
private void Property_IsTiled(ActiveXControl c)
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
            Assert.AreEqual(&quot;MS Sans Serif&quot;, control.Font.Name);
            //Assert.AreEqual(92.2393700787402, control.Width);
            //Assert.AreEqual(43.5118110236221, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


