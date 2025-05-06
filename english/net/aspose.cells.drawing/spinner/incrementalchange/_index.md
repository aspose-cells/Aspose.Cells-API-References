---
title: Spinner.IncrementalChange
second_title: Aspose.Cells for .NET API Reference
description: Spinner property. Gets or sets the amount that the scroll bar or spinner is incremented a line scroll
type: docs
url: /net/aspose.cells.drawing/spinner/incrementalchange/
---
## Spinner.IncrementalChange property

Gets or sets the amount that the scroll bar or spinner is incremented a line scroll.

```csharp
public int IncrementalChange { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(spinnerSrc.IncrementalChange, spinnerDest.IncrementalChange, info + &amp;quot;.IncrementalChange&amp;quot;);
public static void Property_IncrementalChange(Spinner spinnerSrc, Spinner spinnerDest, string info)
        {
            if (AssertHelper.checkNull(spinnerSrc, spinnerDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(spinnerSrc.MsoDrawingType, spinnerDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(spinnerSrc.UpperLeftRow, spinnerDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(spinnerSrc.UpperLeftColumn, spinnerDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(spinnerSrc.LowerRightRow, spinnerDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(spinnerSrc.LowerRightColumn, spinnerDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            //===size===//
            AssertHelper.AreEqual(spinnerSrc.HeightCM, spinnerDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(spinnerSrc.WidthCM, spinnerDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(spinnerSrc.HeightScale, spinnerDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(spinnerSrc.WidthScale, spinnerDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(spinnerSrc.IsLockAspectRatio, spinnerDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protetion===//
            AssertHelper.AreEqual(spinnerSrc.IsLocked, spinnerDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(spinnerSrc.Placement, spinnerDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(spinnerSrc.IsPrintable, spinnerDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web===//
            AssertHelper.AreEqual(spinnerSrc.AlternativeText, spinnerDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===control===//
            AssertHelper.AreEqual(spinnerSrc.CurrentValue, spinnerDest.CurrentValue, info + &quot;.CurrentValue&quot;);
            AssertHelper.AreEqual(spinnerSrc.Min, spinnerDest.Min, info + &quot;.Min&quot;);
            AssertHelper.AreEqual(spinnerSrc.Max, spinnerDest.Max, info + &quot;.Max&quot;);
            AssertHelper.AreEqual(spinnerSrc.IncrementalChange, spinnerDest.IncrementalChange, info + &quot;.IncrementalChange&quot;);
            AssertHelper.AreEqual(spinnerSrc.LinkedCell, spinnerDest.LinkedCell, info + &quot;.LinkedCell&quot;);
            AssertHelper.AreEqual(spinnerSrc.Shadow, spinnerDest.Shadow, info + &quot;.Shadow&quot;);
            //other
            AssertHelper.AreEqual(spinnerSrc.IsHidden, spinnerDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(spinnerSrc.IsGroup, spinnerDest.IsGroup, info + &quot;.IsGroup&quot;);
        }
```

### See Also

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


