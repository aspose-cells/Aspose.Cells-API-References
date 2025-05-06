---
title: LineShape.BeginArrowheadWidth
second_title: Aspose.Cells for .NET API Reference
description: LineShape property. Gets and sets the begin arrow head width of the line
type: docs
url: /net/aspose.cells.drawing/lineshape/beginarrowheadwidth/
---
## LineShape.BeginArrowheadWidth property

Gets and sets the begin arrow head width of the line.

```csharp
[Obsolete("Use Shape.Line.BeginArrowheadWidth property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line.BeginArrowheadWidth property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadWidth, lineshapeDest.BeginArrowheadWidth, info + &amp;quot;.BeginArrowheadWidth&amp;quot;);
public static void Property_BeginArrowheadWidth(LineShape lineshapeSrc, LineShape lineshapeDest, string info)
        {
            if (AssertHelper.checkNull(lineshapeSrc, lineshapeDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(lineshapeSrc.AutoShapeType, lineshapeDest.AutoShapeType, info + &quot;.AutoShapeType&quot;);
            AssertHelper.AreEqual(lineshapeSrc.UpperLeftRow, lineshapeDest.UpperLeftRow, info + &quot;.UpperLeftRow&quot;);
            AssertHelper.AreEqual(lineshapeSrc.UpperLeftColumn, lineshapeDest.UpperLeftColumn, info + &quot;.UpperLeftColumn&quot;);
            AssertHelper.AreEqual(lineshapeSrc.LowerRightRow, lineshapeDest.LowerRightRow, info + &quot;.LowerRightRow&quot;);
            AssertHelper.AreEqual(lineshapeSrc.LowerRightColumn, lineshapeDest.LowerRightColumn, info + &quot;.LowerRightColumn&quot;);  
            //================these properties are supported in excel 2003 format=======================//
            //===colors and lines===//
            MsoFillFormatTest.Property_BeginArrowheadWidth(lineshapeSrc.FillFormat, lineshapeDest.FillFormat, info+&quot;.FillFormat&quot;);
            MsoLineFormatTest.Property_BeginArrowheadWidth(lineshapeSrc.LineFormat, lineshapeDest.LineFormat, info+&quot;.LineFormat&quot;);
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadStyle, lineshapeDest.BeginArrowheadStyle, info + &quot;.BeginArrowheadStyle&quot;);
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadLength, lineshapeDest.BeginArrowheadLength, info + &quot;.BeginArrowheadLength&quot;);
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadWidth, lineshapeDest.BeginArrowheadWidth, info + &quot;.BeginArrowheadWidth&quot;);
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadStyle, lineshapeDest.EndArrowheadStyle, info + &quot;.EndArrowheadStyle&quot;);
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadLength, lineshapeDest.EndArrowheadLength, info + &quot;.EndArrowheadLength&quot;);
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadWidth, lineshapeDest.EndArrowheadWidth, info + &quot;.EndArrowheadWidth&quot;);
            //===size===//
            AssertHelper.AreEqual(lineshapeSrc.HeightCM, lineshapeDest.HeightCM, info + &quot;.HeightCM&quot;);
            AssertHelper.AreEqual(lineshapeSrc.WidthCM, lineshapeDest.WidthCM, info + &quot;.WidthCM&quot;);
            AssertHelper.AreEqual(lineshapeSrc.RotationAngle, lineshapeDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            AssertHelper.AreEqual(lineshapeSrc.HeightScale, lineshapeDest.HeightScale, info + &quot;.HeightScale&quot;);
            AssertHelper.AreEqual(lineshapeSrc.WidthScale, lineshapeDest.WidthScale, info + &quot;.WidthScale&quot;);
            AssertHelper.AreEqual(lineshapeSrc.IsLockAspectRatio, lineshapeDest.IsLockAspectRatio, info + &quot;.IsLockAspectRatio&quot;);
            //===protection===//
            AssertHelper.AreEqual(lineshapeSrc.IsLocked, lineshapeDest.IsLocked, info + &quot;.IsLocked&quot;);
            //===properties===//
            AssertHelper.AreEqual(lineshapeSrc.Placement, lineshapeDest.Placement, info + &quot;.Placement&quot;);
            AssertHelper.AreEqual(lineshapeSrc.IsPrintable, lineshapeDest.IsPrintable, info + &quot;.IsPrintable&quot;);
            //===web===//
            AssertHelper.AreEqual(lineshapeSrc.AlternativeText, lineshapeDest.AlternativeText, info + &quot;.AlternativeText&quot;);
            //===other===//
            AssertHelper.AreEqual(lineshapeSrc.IsHidden, lineshapeDest.IsHidden, info + &quot;.IsHidden&quot;);
            AssertHelper.AreEqual(lineshapeSrc.IsGroup, lineshapeDest.IsGroup, info + &quot;.IsGroup&quot;);
            HyperlinksTest.Property_BeginArrowheadWidth(lineshapeSrc.Hyperlink, lineshapeDest.Hyperlink, info + &quot;.Hyperlink&quot;);
        }
```

### See Also

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


