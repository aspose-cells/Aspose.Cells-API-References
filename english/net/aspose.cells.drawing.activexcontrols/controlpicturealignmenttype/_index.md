---
title: Enum ControlPictureAlignmentType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.ActiveXControls.ControlPictureAlignmentType enum. Represents the alignment of the picture inside the Form or Image
type: docs
url: /net/aspose.cells.drawing.activexcontrols/controlpicturealignmenttype/
---
## ControlPictureAlignmentType enumeration

Represents the alignment of the picture inside the Form or Image.

```csharp
public enum ControlPictureAlignmentType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| TopLeft | `0` | The top left corner. |
| TopRight | `1` | The top right corner. |
| Center | `2` | The center. |
| BottomLeft | `3` | The bottom left corner. |
| BottomRight | `4` | The bottom right corner. |

### Examples

```csharp
// Called: Assert.AreEqual(ControlPictureAlignmentType.Center, control.PictureAlignment);
private void Type_ControlPictureAlignmentType(ActiveXControl c)
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

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


