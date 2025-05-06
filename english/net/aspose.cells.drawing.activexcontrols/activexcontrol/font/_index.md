---
title: ActiveXControl.Font
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Represents the font of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Represents the font of the control.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Calibri&amp;quot;, control.Font.Name);
private void Property_Font(ActiveXControl c)
        {
            TextBoxActiveXControl control = (TextBoxActiveXControl)c;
            Assert.AreEqual(ControlType.TextBox, control.Type);
            Assert.AreEqual(ControlBorderType.None, control.BorderStyle);
            Assert.AreEqual(-2147483642, control.BorderOleColor);
            Assert.AreEqual(ControlSpecialEffectType.Sunken, control.SpecialEffect);
            Assert.AreEqual(0, control.MaxLength);
            Assert.AreEqual(ControlScrollBarType.None, control.ScrollBars);
            Assert.AreEqual((char)0, control.PasswordChar);
            Assert.AreEqual(true, control.IsEditable);
            Assert.AreEqual(true, control.IntegralHeight);
            Assert.AreEqual(false, control.IsDragBehaviorEnabled);
            Assert.AreEqual(false, control.EnterKeyBehavior);
            Assert.AreEqual(false, control.EnterFieldBehavior);
            Assert.AreEqual(false, control.TabKeyBehavior);
            Assert.AreEqual(true, control.HideSelection);
            Assert.AreEqual(false, control.IsAutoTab);
            Assert.AreEqual(false, control.IsMultiLine);
            Assert.AreEqual(false, control.IsAutoWordSelected);
            Assert.AreEqual(true, control.IsWordWrapped);
            Assert.AreEqual(null, control.Text);
            Assert.AreEqual(true, control.IsEnabled);
           // Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual(&quot;Calibri&quot;, control.Font.Name);
            //Assert.AreEqual(75.0047244094488, control.Width);
            //Assert.AreEqual(39.7417322834646, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


