---
title: ScrollBar.CurrentValue
second_title: Aspose.Cells for .NET API Reference
description: ScrollBar property. Gets or sets the current value
type: docs
url: /net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

Gets or sets the current value.

```csharp
public int CurrentValue { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(scrollbarSrc.CurrentValue, scrollbarDest.CurrentValue, info + ".CurrentValue");
public static void ScrollBar_Property_CurrentValue(ScrollBar scrollbarSrc, ScrollBar scrollbarDest, string info)
        {
            if (AssertHelper.checkNull(scrollbarSrc, scrollbarDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(scrollbarSrc.MsoDrawingType, scrollbarDest.MsoDrawingType, info + ".MsoDrawingType");
            AssertHelper.AreEqual(scrollbarSrc.UpperLeftRow, scrollbarDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(scrollbarSrc.UpperLeftColumn, scrollbarDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(scrollbarSrc.LowerRightRow, scrollbarDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(scrollbarSrc.LowerRightColumn, scrollbarDest.LowerRightColumn, info + ".LowerRightColumn");
            //===size===//
            AssertHelper.AreEqual(scrollbarSrc.HeightCM, scrollbarDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(scrollbarSrc.WidthCM, scrollbarDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(scrollbarSrc.HeightScale, scrollbarDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(scrollbarSrc.WidthScale, scrollbarDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(scrollbarSrc.IsLockAspectRatio, scrollbarDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(scrollbarSrc.IsLocked, scrollbarDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(scrollbarSrc.Placement, scrollbarDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(scrollbarSrc.IsPrintable, scrollbarDest.IsPrintable, info + ".IsPrintable");
            //===web====//
            AssertHelper.AreEqual(scrollbarSrc.AlternativeText, scrollbarDest.AlternativeText, info + ".AlternativeText");
            //===control===//
            AssertHelper.AreEqual(scrollbarSrc.CurrentValue, scrollbarDest.CurrentValue, info + ".CurrentValue");
            AssertHelper.AreEqual(scrollbarSrc.Min, scrollbarDest.Min, info + ".Min");
            AssertHelper.AreEqual(scrollbarSrc.Max, scrollbarDest.Max, info + ".Max");
            AssertHelper.AreEqual(scrollbarSrc.IncrementalChange, scrollbarDest.IncrementalChange, info + ".IncrementalChange");
            AssertHelper.AreEqual(scrollbarSrc.PageChange, scrollbarDest.PageChange, info + ".PageChange");
            AssertHelper.AreEqual(scrollbarSrc.LinkedCell, scrollbarDest.LinkedCell, info + ".LinkedCell");
            AssertHelper.AreEqual(scrollbarSrc.Shadow, scrollbarDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(scrollbarSrc.IsHidden, scrollbarDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(scrollbarSrc.IsGroup, scrollbarDest.IsGroup, info + ".IsGroup");
            AssertHelper.AreEqual(scrollbarSrc.LeftCM, scrollbarDest.LeftCM, info + ".LeftCM");
            AssertHelper.AreEqual(scrollbarSrc.TopCM, scrollbarDest.TopCM, info + ".TopCM");
        }
```

### See Also

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


