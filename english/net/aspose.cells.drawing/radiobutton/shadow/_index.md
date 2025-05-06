---
title: RadioButton.Shadow
second_title: Aspose.Cells for .NET API Reference
description: RadioButton property. Indicates whether the combobox has 3D shading
type: docs
url: /net/aspose.cells.drawing/radiobutton/shadow/
---
## RadioButton.Shadow property

Indicates whether the combobox has 3-D shading.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(rbuttonSrc.Shadow, rbuttonDest.Shadow, info + &amp;quot;.Shadow&amp;quot;);
public static void Property_Shadow(RadioButton rbuttonSrc, RadioButton rbuttonDest, string info)
        {
            if (AssertHelper.checkNull(rbuttonSrc, rbuttonDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(rbuttonSrc.MsoDrawingType, rbuttonDest.MsoDrawingType, info + &quot;.MsoDrawingType&quot;);
            AssertHelper.AreEqual(rbuttonSrc.UpperLeftRow, rbuttonDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(rbuttonSrc.UpperLeftColumn, rbuttonDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(rbuttonSrc.LowerRightRow, rbuttonDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(rbuttonSrc.LowerRightColumn, rbuttonDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            AssertHelper.AreEqual(rbuttonSrc.Text, rbuttonDest.Text, info + &quot;.Text&quot;);
            //===colors and lines===//
            MsoFillFormatTest.Property_Shadow(rbuttonSrc.FillFormat, rbuttonDest.FillFormat, info + &quot;.FillFormat&quot;);
            MsoLineFormatTest.Property_Shadow(rbuttonSrc.LineFormat, rbuttonDest.LineFormat, info + &quot;.LineFormat&quot;);           
            //===size===//
            AssertHelper.AreEqual(rbuttonSrc.HeightCM, rbuttonDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(rbuttonSrc.WidthCM, rbuttonDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(rbuttonSrc.HeightScale, rbuttonDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(rbuttonSrc.WidthScale, rbuttonDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(rbuttonSrc.IsLockAspectRatio, rbuttonDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection====//
            AssertHelper.AreEqual(rbuttonSrc.IsLocked, rbuttonDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(rbuttonSrc.Placement, rbuttonDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(rbuttonSrc.IsPrintable, rbuttonDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web===//
            AssertHelper.AreEqual(rbuttonSrc.AlternativeText, rbuttonDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===control===//
            AssertHelper.AreEqual(rbuttonSrc.IsChecked, rbuttonDest.IsChecked, info + &quot;.IsChecked&quot;);
            AssertHelper.AreEqual(rbuttonSrc.LinkedCell, rbuttonDest.LinkedCell, info + &quot;.LinkedCell&quot;);
            AssertHelper.AreEqual(rbuttonSrc.Shadow, rbuttonDest.Shadow, info + &quot;.Shadow&quot;);
            //other
            AssertHelper.AreEqual(rbuttonSrc.IsHidden, rbuttonDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(rbuttonSrc.IsGroup, rbuttonDest.IsGroup, info + &quot;.IsGroup&quot;);

            AssertHelper.AreEqual(rbuttonSrc.LeftCM, rbuttonDest.LeftCM, info + &quot;.LeftCM&quot;);
            AssertHelper.AreEqual(rbuttonSrc.TopCM, rbuttonDest.TopCM, info + &quot;.TopCM&quot;);
        }
```

### See Also

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


