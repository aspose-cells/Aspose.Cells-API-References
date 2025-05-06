---
title: ListBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Indicates whether the combobox has 3D shading
type: docs
url: /net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

Indicates whether the combobox has 3-D shading.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(listboxSrc.Shadow, listboxDest.Shadow, info + &amp;quot;.Shadow&amp;quot;);
public static void Property_Shadow(ListBox listboxSrc, ListBox listboxDest, string info)
        {
            if (AssertHelper.checkNull(listboxSrc, listboxDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format====================//
            AssertHelper.AreEqual(listboxSrc.MsoDrawingType, listboxDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(listboxSrc.UpperLeftRow, listboxDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(listboxSrc.UpperLeftColumn, listboxDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(listboxSrc.LowerRightRow, listboxDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(listboxSrc.LowerRightColumn, listboxDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);  
            //===size===//
            AssertHelper.AreEqual(listboxSrc.HeightCM, listboxDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(listboxSrc.WidthCM, listboxDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(listboxSrc.HeightScale, listboxDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(listboxSrc.WidthScale, listboxDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(listboxSrc.IsLockAspectRatio, listboxDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(listboxSrc.IsLocked, listboxDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(listboxSrc.Placement, listboxDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(listboxSrc.IsPrintable, listboxDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web===//
            AssertHelper.AreEqual(listboxSrc.AlternativeText, listboxDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===control===//
            AssertHelper.AreEqual(listboxSrc.InputRange, listboxDest.InputRange, info + &quot;.InputRange&quot;);
            AssertHelper.AreEqual(listboxSrc.LinkedCell, listboxDest.LinkedCell, info + &quot;.LinkedCell&quot;);
            AssertHelper.AreEqual(listboxSrc.SelectionType, listboxDest.SelectionType, info + &quot;.SelectionType&quot;);
            AssertHelper.AreEqual(listboxSrc.Shadow, listboxDest.Shadow, info + &quot;.Shadow&quot;);
            //other
            AssertHelper.AreEqual(listboxSrc.IsHidden, listboxDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(listboxSrc.IsGroup, listboxDest.IsGroup, info + &quot;.IsGroup&quot;);

            AssertHelper.AreEqual(listboxSrc.ItemCount, listboxDest.ItemCount, info + &quot;.ItemCount&quot;);
            AssertHelper.AreEqual(listboxSrc.SelectedIndex, listboxDest.SelectedIndex, info + &quot;.SelectedIndex&quot;);
        }
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


