---
title: LineShape.EndArrowheadLength
second_title: Aspose.Cells for .NET API Reference
description: LineShape property. Gets and sets the end arrow head length of the line
type: docs
url: /net/aspose.cells.drawing/lineshape/endarrowheadlength/
---
## LineShape.EndArrowheadLength property

Gets and sets the end arrow head length of the line.

```csharp
[Obsolete("Use Shape.Line.EndArrowheadLength property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line.EndArrowheadLength property. This property will be removed 12 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(lineshapeSrc.EndArrowheadLength, lineshapeDest.EndArrowheadLength, info + ".EndArrowheadLength");
public static void LineShape_Property_EndArrowheadLength(LineShape lineshapeSrc, LineShape lineshapeDest, string info)
        {
            if (AssertHelper.checkNull(lineshapeSrc, lineshapeDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(lineshapeSrc.AutoShapeType, lineshapeDest.AutoShapeType, info + ".AutoShapeType");
            AssertHelper.AreEqual(lineshapeSrc.UpperLeftRow, lineshapeDest.UpperLeftRow, info + ".UpperLeftRow");
            AssertHelper.AreEqual(lineshapeSrc.UpperLeftColumn, lineshapeDest.UpperLeftColumn, info + ".UpperLeftColumn");
            AssertHelper.AreEqual(lineshapeSrc.LowerRightRow, lineshapeDest.LowerRightRow, info + ".LowerRightRow");
            AssertHelper.AreEqual(lineshapeSrc.LowerRightColumn, lineshapeDest.LowerRightColumn, info + ".LowerRightColumn");  
            //================these properties are supported in excel 2003 format=======================//
            //===colors and lines===//
            MsoFillFormatTest.LineShape_Property_EndArrowheadLength(lineshapeSrc.FillFormat, lineshapeDest.FillFormat, info+".FillFormat");
            MsoLineFormatTest.LineShape_Property_EndArrowheadLength(lineshapeSrc.LineFormat, lineshapeDest.LineFormat, info+".LineFormat");
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadStyle, lineshapeDest.BeginArrowheadStyle, info + ".BeginArrowheadStyle");
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadLength, lineshapeDest.BeginArrowheadLength, info + ".BeginArrowheadLength");
            AssertHelper.AreEqual(lineshapeSrc.BeginArrowheadWidth, lineshapeDest.BeginArrowheadWidth, info + ".BeginArrowheadWidth");
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadStyle, lineshapeDest.EndArrowheadStyle, info + ".EndArrowheadStyle");
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadLength, lineshapeDest.EndArrowheadLength, info + ".EndArrowheadLength");
            AssertHelper.AreEqual(lineshapeSrc.EndArrowheadWidth, lineshapeDest.EndArrowheadWidth, info + ".EndArrowheadWidth");
            //===size===//
            AssertHelper.AreEqual(lineshapeSrc.HeightCM, lineshapeDest.HeightCM, info + ".HeightCM");
            AssertHelper.AreEqual(lineshapeSrc.WidthCM, lineshapeDest.WidthCM, info + ".WidthCM");
            AssertHelper.AreEqual(lineshapeSrc.RotationAngle, lineshapeDest.RotationAngle, info + ".RotationAngle");
            AssertHelper.AreEqual(lineshapeSrc.HeightScale, lineshapeDest.HeightScale, info + ".HeightScale");
            AssertHelper.AreEqual(lineshapeSrc.WidthScale, lineshapeDest.WidthScale, info + ".WidthScale");
            AssertHelper.AreEqual(lineshapeSrc.IsLockAspectRatio, lineshapeDest.IsLockAspectRatio, info + ".IsLockAspectRatio");
            //===protection===//
            AssertHelper.AreEqual(lineshapeSrc.IsLocked, lineshapeDest.IsLocked, info + ".IsLocked");
            //===properties===//
            AssertHelper.AreEqual(lineshapeSrc.Placement, lineshapeDest.Placement, info + ".Placement");
            AssertHelper.AreEqual(lineshapeSrc.IsPrintable, lineshapeDest.IsPrintable, info + ".IsPrintable");
            //===web===//
            AssertHelper.AreEqual(lineshapeSrc.AlternativeText, lineshapeDest.AlternativeText, info + ".AlternativeText");
            //===other===//
            AssertHelper.AreEqual(lineshapeSrc.IsHidden, lineshapeDest.IsHidden, info + ".IsHidden");
            AssertHelper.AreEqual(lineshapeSrc.IsGroup, lineshapeDest.IsGroup, info + ".IsGroup");
            HyperlinksTest.LineShape_Property_EndArrowheadLength(lineshapeSrc.Hyperlink, lineshapeDest.Hyperlink, info + ".Hyperlink");
        }
```

### See Also

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


