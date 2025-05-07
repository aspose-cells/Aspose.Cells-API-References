---
title: ActiveXControl.IsAutoSize
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Indicates whether the control will automatically resize to display its entire contents
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/
---
## ActiveXControl.IsAutoSize property

Indicates whether the control will automatically resize to display its entire contents.

```csharp
public virtual bool IsAutoSize { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, control.IsAutoSize);
private void Property_IsAutoSize(ActiveXControl c)
        {
            SpinButtonActiveXControl control = (SpinButtonActiveXControl)c;
            Assert.AreEqual(ControlType.SpinButton, control.Type);
            Assert.AreEqual(0, control.Min);
            Assert.AreEqual(100, control.Max);
            Assert.AreEqual(0, control.Position);
            Assert.AreEqual(1, control.SmallChange);
            Assert.AreEqual(ControlScrollOrientation.Auto, control.Orientation);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("MS Sans Serif", control.Font.Name);
            //Assert.AreEqual(53.2629921259842, control.Width);
            //Assert.AreEqual(44.2488188976378, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


