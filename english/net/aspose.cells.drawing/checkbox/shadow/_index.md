---
title: CheckBox.Shadow
second_title: Aspose.Cells for .NET API Reference
description: CheckBox property. Indicates whether the combobox has 3D shading
type: docs
url: /net/aspose.cells.drawing/checkbox/shadow/
---
## CheckBox.Shadow property

Indicates whether the combobox has 3-D shading.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cbSrc.Shadow, cbDest.Shadow, info + ".Shadow");
public static void CheckBox_Property_Shadow(CheckBox cbSrc, CheckBox cbDest, string info)
        {
            if (AssertHelper.checkNull(cbSrc, cbDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(cbSrc.AutoShapeType, cbDest.AutoShapeType, info + ".AutoShapeType");
            AssertHelper.AreEqual(cbSrc.UpperLeftRow, cbDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(cbSrc.UpperLeftColumn, cbDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(cbSrc.LowerRightRow, cbDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(cbSrc.LowerRightColumn, cbDest.LowerRightColumn, info + ".LowerRightColumn");
            AssertHelper.AreEqual(cbSrc.Text, cbDest.Text, info + ".Text");
            AssertHelper.AreEqual(cbSrc.Value, cbDest.Value, info + ".Value");
            //===============these properties are supported in excel 2003 format==============//
            //===colors and lines===//
            MsoFillFormatTest.CheckBox_Property_Shadow(cbSrc.FillFormat, cbDest.FillFormat, info + ".FillFormat");
            MsoLineFormatTest.CheckBox_Property_Shadow(cbSrc.LineFormat, cbDest.LineFormat, info + ".LineFormat");
            //===size===//
            AssertHelper.AreEqual(cbSrc.Height, cbDest.Height, info + ".Height");
            AssertHelper.AreEqual(cbSrc.Width, cbDest.Width, info + ".Width");
            AssertHelper.AreEqual(cbSrc.HeightScale, cbDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(cbSrc.WidthScale, cbDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(cbSrc.IsLockAspectRatio, cbDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(cbSrc.IsLocked, cbDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(cbSrc.Placement, cbDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(cbSrc.IsPrintable, cbDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(cbSrc.AlternativeText, cbDest.AlternativeText, info + ".AlternativeText");
            //===Control===//
            AssertHelper.AreEqual(cbSrc.CheckedValue, cbDest.CheckedValue, info + ".CheckValue");
            AssertHelper.AreEqual(cbSrc.LinkedCell, cbDest.LinkedCell, info + ".CheckValue");
            AssertHelper.AreEqual(cbSrc.Shadow, cbDest.Shadow, info + ".Shadow");
            //other        
            AssertHelper.AreEqual(cbSrc.IsHidden, cbDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(cbSrc.IsGroup, cbDest.IsGroup, info + ".IsGroup");
        }
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


