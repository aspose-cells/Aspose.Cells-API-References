---
title: ComboBoxActiveXControl.EnterFieldBehavior
second_title: Aspose.Cells for .NET API Reference
description: ComboBoxActiveXControl property. Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/enterfieldbehavior/
---
## ComboBoxActiveXControl.EnterFieldBehavior property

Specifies selection behavior when entering the control. True specifies that the selection remains unchanged from last time the control was active. False specifies that all the text in the control will be selected when entering the control.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, control.EnterFieldBehavior);
private void Property_EnterFieldBehavior(ActiveXControl c)
        {
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)c;
            Assert.AreEqual(ControlType.ComboBox, control.Type);
            Assert.AreEqual(0, control.ListWidth);
            Assert.AreEqual(1, control.BoundColumn);
            Assert.AreEqual(-1, control.TextColumn);
            Assert.AreEqual(1, control.ColumnCount);
            Assert.AreEqual(8, control.ListRows);
            Assert.AreEqual(ControlMatchEntryType.Complete, control.MatchEntry);
            Assert.AreEqual(ControlListStyle.Plain, control.ListStyle);
            Assert.AreEqual(ControlBorderType.None, control.BorderStyle);
            Assert.AreEqual(-2147483642, control.BorderOleColor);
            Assert.AreEqual(ControlSpecialEffectType.Sunken, control.SpecialEffect);
            Assert.AreEqual(true, control.IsEditable);
            Assert.AreEqual(false, control.ShowColumnHeads);
            Assert.AreEqual(false, control.IsDragBehaviorEnabled);
            Assert.AreEqual(false, control.EnterFieldBehavior);
            Assert.AreEqual(false, control.IsAutoWordSelected);
            Assert.AreEqual(true, control.SelectionMargin);
            Assert.AreEqual(true, control.IsEnabled);
            //Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(82.488188976378, control.Width);
            //Assert.AreEqual(32.9952755905512, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


