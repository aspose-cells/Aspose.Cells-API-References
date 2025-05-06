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
            CheckBoxActiveXControl control = (CheckBoxActiveXControl)c;
            Assert.AreEqual(ControlType.CheckBox, control.Type);
            Assert.AreEqual(&quot;Sheet1&quot;, control.GroupName);
            Assert.AreEqual(ControlCaptionAlignmentType.Right, control.Alignment);
            Assert.AreEqual(true, control.IsWordWrapped);
            Assert.AreEqual(CheckValueType.UnChecked, control.Value);
            Assert.AreEqual(true, control.IsEnabled);
           // Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual(&quot;Calibri&quot;, control.Font.Name);
            //Assert.AreEqual(114.009448818898, control.Width);
            //Assert.AreEqual(65.9905511811024, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


