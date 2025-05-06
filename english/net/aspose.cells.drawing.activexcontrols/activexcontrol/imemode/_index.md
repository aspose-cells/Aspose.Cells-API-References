---
title: ActiveXControl.IMEMode
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Gets and sets the default runtime mode of the Input Method Editor for the control as it receives focus
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Gets and sets the default run-time mode of the Input Method Editor for the control as it receives focus.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
private void Property_IMEMode(ActiveXControl c)
        {
            ScrollBarActiveXControl control = (ScrollBarActiveXControl)c;
            Assert.AreEqual(ControlType.ScrollBar, control.Type);
            Assert.AreEqual(1, control.LargeChange);
            Assert.AreEqual(0, control.Min);
            Assert.AreEqual(32767, control.Max);
            Assert.AreEqual(0, control.Position);
            Assert.AreEqual(1, control.SmallChange);
            Assert.AreEqual(ControlScrollOrientation.Auto, control.Orientation);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual(&quot;MS Sans Serif&quot;, control.Font.Name);
            //Assert.AreEqual(45.7511811023622, control.Width);
            //Assert.AreEqual(34.4976377952756, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483633, control.BackOleColor);
        }
```

### See Also

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


