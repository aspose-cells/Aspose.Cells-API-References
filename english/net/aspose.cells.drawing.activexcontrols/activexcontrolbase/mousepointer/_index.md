---
title: ActiveXControlBase.MousePointer
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the type of icon displayed as the mouse pointer for the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Gets and sets the type of icon displayed as the mouse pointer for the control.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
private void Property_MousePointer(ActiveXControl c)
        {
            CommandButtonActiveXControl control = (CommandButtonActiveXControl)c;
            Assert.AreEqual(ControlType.CommandButton, control.Type);
            Assert.AreEqual(&quot;CommandButton1&quot;, control.Caption);
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
            Assert.AreEqual(&quot;Calibri&quot;, control.Font.Name);
            //Assert.AreEqual(85.4929133858268, control.Width);
            //Assert.AreEqual(31.4929133858268, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


