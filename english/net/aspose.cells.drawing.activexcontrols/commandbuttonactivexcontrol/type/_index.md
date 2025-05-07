---
title: CommandButtonActiveXControl.Type
second_title: Aspose.Cells for .NET API Reference
description: CommandButtonActiveXControl property. Gets the type of the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/
---
## CommandButtonActiveXControl.Type property

Gets the type of the ActiveX control.

```csharp
public override ControlType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ControlType.CommandButton, control.Type);
private void Property_Type(ActiveXControl c)
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

* enum [ControlType](../../controltype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


