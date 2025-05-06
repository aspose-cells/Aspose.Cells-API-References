---
title: CheckBoxActiveXControl.Type
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxActiveXControl property. Gets the type of the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

Gets the type of the ActiveX control.

```csharp
public override ControlType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ControlType.CheckBox, control.Type);
private void Property_Type(ActiveXControl c)
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

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


