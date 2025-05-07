---
title: ListBox.SelectionType
second_title: Aspose.Cells for .NET API Reference
description: ListBox property. Gets or sets the selection mode of the specified list box
type: docs
url: /net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Gets or sets the selection mode of the specified list box.

```csharp
public SelectionType SelectionType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(listboxSrc.SelectionType, listboxDest.SelectionType, info + ".SelectionType");
public static void Property_SelectionType(ListBox listboxSrc, ListBox listboxDest, string info)
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

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


