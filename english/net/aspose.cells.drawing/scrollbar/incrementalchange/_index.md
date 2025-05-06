---
title: ScrollBar.IncrementalChange
second_title: Aspose.Cells for .NET API Reference
description: ScrollBar property. Gets or sets the amount that the scroll bar or spinner is incremented a line scroll
type: docs
url: /net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Gets or sets the amount that the scroll bar or spinner is incremented a line scroll.

```csharp
public int IncrementalChange { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(scrollbarSrc.IncrementalChange, scrollbarDest.IncrementalChange, info + &amp;quot;.IncrementalChange&amp;quot;);
public static void Property_IncrementalChange(ScrollBar scrollbarSrc, ScrollBar scrollbarDest, string info)
        {
            if (AssertHelper.checkNull(scrollbarSrc, scrollbarDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(scrollbarSrc.MsoDrawingType, scrollbarDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(scrollbarSrc.UpperLeftRow, scrollbarDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(scrollbarSrc.UpperLeftColumn, scrollbarDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(scrollbarSrc.LowerRightRow, scrollbarDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(scrollbarSrc.LowerRightColumn, scrollbarDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            //===size===//
            AssertHelper.AreEqual(scrollbarSrc.HeightCM, scrollbarDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(scrollbarSrc.WidthCM, scrollbarDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(scrollbarSrc.HeightScale, scrollbarDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(scrollbarSrc.WidthScale, scrollbarDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(scrollbarSrc.IsLockAspectRatio, scrollbarDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(scrollbarSrc.IsLocked, scrollbarDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(scrollbarSrc.Placement, scrollbarDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(scrollbarSrc.IsPrintable, scrollbarDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web====//
            AssertHelper.AreEqual(scrollbarSrc.AlternativeText, scrollbarDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===control===//
            AssertHelper.AreEqual(scrollbarSrc.CurrentValue, scrollbarDest.CurrentValue, info + &quot;.CurrentValue&quot;);
            AssertHelper.AreEqual(scrollbarSrc.Min, scrollbarDest.Min, info + &quot;.Min&quot;);
            AssertHelper.AreEqual(scrollbarSrc.Max, scrollbarDest.Max, info + &quot;.Max&quot;);
            AssertHelper.AreEqual(scrollbarSrc.IncrementalChange, scrollbarDest.IncrementalChange, info + &quot;.IncrementalChange&quot;);
            AssertHelper.AreEqual(scrollbarSrc.PageChange, scrollbarDest.PageChange, info + &quot;.PageChange&quot;);
            AssertHelper.AreEqual(scrollbarSrc.LinkedCell, scrollbarDest.LinkedCell, info + &quot;.LinkedCell&quot;);
            AssertHelper.AreEqual(scrollbarSrc.Shadow, scrollbarDest.Shadow, info + &quot;.Shadow&quot;);
            //other
            AssertHelper.AreEqual(scrollbarSrc.IsHidden, scrollbarDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(scrollbarSrc.IsGroup, scrollbarDest.IsGroup, info + &quot;.IsGroup&quot;);
            AssertHelper.AreEqual(scrollbarSrc.LeftCM, scrollbarDest.LeftCM, info + &quot;.LeftCM&quot;);
            AssertHelper.AreEqual(scrollbarSrc.TopCM, scrollbarDest.TopCM, info + &quot;.TopCM&quot;);
        }
```

### See Also

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


