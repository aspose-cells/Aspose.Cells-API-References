---
title: CommandButtonActiveXControl.Picture
second_title: Aspose.Cells for .NET API Reference
description: CommandButtonActiveXControl property. Gets and sets the data of the picture
type: docs
url: /net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

Gets and sets the data of the picture.

```csharp
public byte[] Picture { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(null, control.Picture);
private void CommandButtonActiveXControl_Property_Picture(ActiveXControl c)
        {
            CommandButtonActiveXControl control = (CommandButtonActiveXControl)c;
            Assert.AreEqual(ControlType.CommandButton, control.Type);
            Assert.AreEqual("CommandButton1", control.Caption);
            Assert.AreEqual(ControlPicturePositionType.AboveCenter, control.PicturePosition);
            Assert.AreEqual(null, control.Picture);
            Assert.AreEqual((char)0, control.Accelerator);
            Assert.AreEqual(false, control.TakeFocusOnClick);
            Assert.AreEqual(false, control.IsWordWrapped);
            Assert.AreEqual(true, control.IsEnabled);
           // Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(85.4929133858268, control.Width);
            //Assert.AreEqual(31.4929133858268, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


