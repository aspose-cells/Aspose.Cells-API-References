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

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


