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
// Called: AssertHelper.AreEqual(cbSrc.Shadow, cbDest.Shadow, info + &amp;quot;.Shadow&amp;quot;);
public static void Property_Shadow(CheckBox cbSrc, CheckBox cbDest, string info)
        {
            if (AssertHelper.checkNull(cbSrc, cbDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(cbSrc.AutoShapeType, cbDest.AutoShapeType, info + &quot;.AutoShapeType&quot;);
            AssertHelper.AreEqual(cbSrc.UpperLeftRow, cbDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(cbSrc.UpperLeftColumn, cbDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(cbSrc.LowerRightRow, cbDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(cbSrc.LowerRightColumn, cbDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);
            AssertHelper.AreEqual(cbSrc.Text, cbDest.Text, info + &quot;.Text&quot;);
            AssertHelper.AreEqual(cbSrc.Value, cbDest.Value, info + &quot;.Value&quot;);
            //===============these properties are supported in excel 2003 format==============//
            //===colors and lines===//
            MsoFillFormatTest.Property_Shadow(cbSrc.FillFormat, cbDest.FillFormat, info + &quot;.FillFormat&quot;);
            MsoLineFormatTest.Property_Shadow(cbSrc.LineFormat, cbDest.LineFormat, info + &quot;.LineFormat&quot;);
            //===size===//
            AssertHelper.AreEqual(cbSrc.Height, cbDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(cbSrc.Width, cbDest.Width, info + &quot;.Width&quot;);
            AssertHelper.AreEqual(cbSrc.HeightScale, cbDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(cbSrc.WidthScale, cbDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(cbSrc.IsLockAspectRatio, cbDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(cbSrc.IsLocked, cbDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(cbSrc.Placement, cbDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(cbSrc.IsPrintable, cbDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web===//
            AssertHelper.AreEqual(cbSrc.AlternativeText, cbDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===Control===//
            AssertHelper.AreEqual(cbSrc.CheckedValue, cbDest.CheckedValue, info + &quot;.CheckValue&quot;);
            AssertHelper.AreEqual(cbSrc.LinkedCell, cbDest.LinkedCell, info + &quot;.CheckValue&quot;);
            AssertHelper.AreEqual(cbSrc.Shadow, cbDest.Shadow, info + &quot;.Shadow&quot;);
            //other        
            AssertHelper.AreEqual(cbSrc.IsHidden, cbDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(cbSrc.IsGroup, cbDest.IsGroup, info + &quot;.IsGroup&quot;);
        }
```

### See Also

* class [CheckBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


