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
// Called: AssertHelper.AreEqual(rbuttonSrc.Shadow, rbuttonDest.Shadow, info + ".Shadow");
public static void Property_Shadow(RadioButton rbuttonSrc, RadioButton rbuttonDest, string info)
        {
            if (AssertHelper.checkNull(rbuttonSrc, rbuttonDest, info))
            {
                return;
            }
            //====================properties are supported in excel 2003 format=======================//
            AssertHelper.AreEqual(rbuttonSrc.MsoDrawingType, rbuttonDest.MsoDrawingType, info + ".MsoDrawingType");
            AssertHelper.AreEqual(rbuttonSrc.UpperLeftRow, rbuttonDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(rbuttonSrc.UpperLeftColumn, rbuttonDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(rbuttonSrc.LowerRightRow, rbuttonDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(rbuttonSrc.LowerRightColumn, rbuttonDest.LowerRightColumn, info + ".LowerRightColumn");
            AssertHelper.AreEqual(rbuttonSrc.Text, rbuttonDest.Text, info + ".Text");
            //===colors and lines===//
            MsoFillFormatTest.Property_Shadow(rbuttonSrc.FillFormat, rbuttonDest.FillFormat, info + ".FillFormat");
            MsoLineFormatTest.Property_Shadow(rbuttonSrc.LineFormat, rbuttonDest.LineFormat, info + ".LineFormat");           
            //===size===//
            AssertHelper.AreEqual(rbuttonSrc.HeightCM, rbuttonDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(rbuttonSrc.WidthCM, rbuttonDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(rbuttonSrc.HeightScale, rbuttonDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(rbuttonSrc.WidthScale, rbuttonDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(rbuttonSrc.IsLockAspectRatio, rbuttonDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection====//
            AssertHelper.AreEqual(rbuttonSrc.IsLocked, rbuttonDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(rbuttonSrc.Placement, rbuttonDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(rbuttonSrc.IsPrintable, rbuttonDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(rbuttonSrc.AlternativeText, rbuttonDest.AlternativeText, info + ".AlternativeText");
            //===control===//
            AssertHelper.AreEqual(rbuttonSrc.IsChecked, rbuttonDest.IsChecked, info + ".IsChecked");
            AssertHelper.AreEqual(rbuttonSrc.LinkedCell, rbuttonDest.LinkedCell, info + ".LinkedCell");
            AssertHelper.AreEqual(rbuttonSrc.Shadow, rbuttonDest.Shadow, info + ".Shadow");
            //other
            AssertHelper.AreEqual(rbuttonSrc.IsHidden, rbuttonDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(rbuttonSrc.IsGroup, rbuttonDest.IsGroup, info + ".IsGroup");

            AssertHelper.AreEqual(rbuttonSrc.LeftCM, rbuttonDest.LeftCM, info + ".LeftCM");
            AssertHelper.AreEqual(rbuttonSrc.TopCM, rbuttonDest.TopCM, info + ".TopCM");
        }
```

### See Also

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


