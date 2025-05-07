---
title: CheckBoxActiveXControl.Value
second_title: Aspose.Cells for .NET API Reference
description: CheckBoxActiveXControl property. Indicates if the control is checked or not
type: docs
url: /net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

Indicates if the control is checked or not.

```csharp
public CheckValueType Value { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CheckValueType.UnChecked, control.Value);
private void Property_Value(ActiveXControl c)
        {
            CheckBoxActiveXControl control = (CheckBoxActiveXControl)c;
            Assert.AreEqual(ControlType.CheckBox, control.Type);
            Assert.AreEqual("Sheet1", control.GroupName);
            Assert.AreEqual(ControlCaptionAlignmentType.Right, control.Alignment);
            Assert.AreEqual(true, control.IsWordWrapped);
            Assert.AreEqual(CheckValueType.UnChecked, control.Value);
            Assert.AreEqual(true, control.IsEnabled);
           // Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(114.009448818898, control.Width);
            //Assert.AreEqual(65.9905511811024, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


