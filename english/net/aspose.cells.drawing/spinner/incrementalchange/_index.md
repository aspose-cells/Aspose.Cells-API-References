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
// Called: AssertHelper.AreEqual(spinnerSrc.IncrementalChange, spinnerDest.IncrementalChange, info + ".IncrementalChange");
public static void Property_IncrementalChange(Spinner spinnerSrc, Spinner spinnerDest, string info)
        {
            if (AssertHelper.checkNull(spinnerSrc, spinnerDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(spinnerSrc.MsoDrawingType, spinnerDest.MsoDrawingType, info + ".MsoDrawingType");
            AssertHelper.AreEqual(spinnerSrc.UpperLeftRow, spinnerDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(spinnerSrc.UpperLeftColumn, spinnerDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(spinnerSrc.LowerRightRow, spinnerDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(spinnerSrc.LowerRightColumn, spinnerDest.LowerRightColumn, info + ".LowerRightColumn");
            //===size===//
            AssertHelper.AreEqual(spinnerSrc.HeightCM, spinnerDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(spinnerSrc.WidthCM, spinnerDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(spinnerSrc.HeightScale, spinnerDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(spinnerSrc.WidthScale, spinnerDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(spinnerSrc.IsLockAspectRatio, spinnerDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protetion===//
            AssertHelper.AreEqual(spinnerSrc.IsLocked, spinnerDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(spinnerSrc.Placement, spinnerDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(spinnerSrc.IsPrintable, spinnerDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(spinnerSrc.AlternativeText, spinnerDest.AlternativeText, info + ".AlternativeText");
            //===control===//
            AssertHelper.AreEqual(spinnerSrc.CurrentValue, spinnerDest.CurrentValue, info + ".CurrentValue");
            AssertHelper.AreEqual(spinnerSrc.Min, spinnerDest.Min, info + ".Min");
            AssertHelper.AreEqual(spinnerSrc.Max, spinnerDest.Max, info + ".Max");
            AssertHelper.AreEqual(spinnerSrc.IncrementalChange, spinnerDest.IncrementalChange, info + ".IncrementalChange");
            AssertHelper.AreEqual(spinnerSrc.LinkedCell, spinnerDest.LinkedCell, info + ".LinkedCell");
            AssertHelper.AreEqual(spinnerSrc.Shadow, spinnerDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(spinnerSrc.IsHidden, spinnerDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(spinnerSrc.IsGroup, spinnerDest.IsGroup, info + ".IsGroup");
        }
```

### See Also

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


