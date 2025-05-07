---
title: ImageActiveXControl.Picture
second_title: Aspose.Cells for .NET API Reference
description: ImageActiveXControl property. Gets and sets the data of the picture
type: docs
url: /net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/
---
## ImageActiveXControl.Picture property

Gets and sets the data of the picture.

```csharp
public byte[] Picture { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(null, control.Picture);
private void Property_Picture(ActiveXControl c)
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

* class [ImageActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


