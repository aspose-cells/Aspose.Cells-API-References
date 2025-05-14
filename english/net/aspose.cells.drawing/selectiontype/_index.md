---
title: Enum SelectionType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.SelectionType enum. The selection type of list box
type: docs
url: /net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

The selection type of list box.

```csharp
public enum SelectionType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Single | `0` | Sigle selection type. |
| Multi | `1` | Multiple selection type. |
| Extend | `2` | Extend selection type. |

### Examples

```csharp
// Called: Assert.AreEqual(SelectionType.Single, control.SelectionType);
private void Drawing_Type_SelectionType(ActiveXControl c)
        {
            ListBoxActiveXControl control = (ListBoxActiveXControl)c;
            Assert.AreEqual(ControlType.ListBox, control.Type);
           // Assert.AreEqual(0, control.MaxLength);
            Assert.AreEqual(ControlScrollBarType.BarsBoth, control.ScrollBars);
            Assert.AreEqual(0, control.ListWidth);
            Assert.AreEqual(1, control.BoundColumn);
            Assert.AreEqual(-1, control.TextColumn);
            Assert.AreEqual(1, control.ColumnCount);
            Assert.AreEqual(ControlMatchEntryType.FirstLetter, control.MatchEntry);
            Assert.AreEqual(ControlListStyle.Plain, control.ListStyle);
            Assert.AreEqual(SelectionType.Single, control.SelectionType);
            Assert.AreEqual(ControlBorderType.None, control.BorderStyle);
            Assert.AreEqual(-2147483642, control.BorderOleColor);
            Assert.AreEqual(ControlSpecialEffectType.Sunken, control.SpecialEffect);
            Assert.AreEqual(false, control.ShowColumnHeads);
            Assert.AreEqual(true, control.IntegralHeight);
            Assert.AreEqual(true, control.IsEnabled);
           // Assert.AreEqual(false, control.IsLocked);
            Assert.AreEqual(false, control.IsTransparent);
            Assert.AreEqual(false, control.IsAutoSize);
            Assert.AreEqual(InputMethodEditorMode.NoControl, control.IMEMode);
            Assert.AreEqual("Calibri", control.Font.Name);
            //Assert.AreEqual(67.4929133858268, control.Width);
            //Assert.AreEqual(21.7417322834646, control.Height);
            Assert.AreEqual(null, control.MouseIcon);
            Assert.AreEqual(ControlMousePointerType.Default, control.MousePointer);
            Assert.AreEqual(-2147483630, control.ForeOleColor);
            Assert.AreEqual(-2147483643, control.BackOleColor);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


