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
// Called: AssertHelper.AreEqual(listboxSrc.Shadow, listboxDest.Shadow, info + ".Shadow");
public static void ListBox_Property_Shadow(ListBox listboxSrc, ListBox listboxDest, string info)
        {
            if (AssertHelper.checkNull(listboxSrc, listboxDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format====================//
            AssertHelper.AreEqual(listboxSrc.MsoDrawingType, listboxDest.MsoDrawingType, info + ".MsoDrawingType");
            AssertHelper.AreEqual(listboxSrc.UpperLeftRow, listboxDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(listboxSrc.UpperLeftColumn, listboxDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(listboxSrc.LowerRightRow, listboxDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(listboxSrc.LowerRightColumn, listboxDest.LowerRightColumn, info + ".LowerRightColumn");  
            //===size===//
            AssertHelper.AreEqual(listboxSrc.HeightCM, listboxDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(listboxSrc.WidthCM, listboxDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(listboxSrc.HeightScale, listboxDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(listboxSrc.WidthScale, listboxDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(listboxSrc.IsLockAspectRatio, listboxDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(listboxSrc.IsLocked, listboxDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(listboxSrc.Placement, listboxDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(listboxSrc.IsPrintable, listboxDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(listboxSrc.AlternativeText, listboxDest.AlternativeText, info + ".AlternativeText");
            //===control===//
            AssertHelper.AreEqual(listboxSrc.InputRange, listboxDest.InputRange, info + ".InputRange");
            AssertHelper.AreEqual(listboxSrc.LinkedCell, listboxDest.LinkedCell, info + ".LinkedCell");
            AssertHelper.AreEqual(listboxSrc.SelectionType, listboxDest.SelectionType, info + ".SelectionType");
            AssertHelper.AreEqual(listboxSrc.Shadow, listboxDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(listboxSrc.IsHidden, listboxDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(listboxSrc.IsGroup, listboxDest.IsGroup, info + ".IsGroup");

            AssertHelper.AreEqual(listboxSrc.ItemCount, listboxDest.ItemCount, info + ".ItemCount");
            AssertHelper.AreEqual(listboxSrc.SelectedIndex, listboxDest.SelectedIndex, info + ".SelectedIndex");
        }
```

### See Also

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


