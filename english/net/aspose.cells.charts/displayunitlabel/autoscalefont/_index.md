---
title: DisplayUnitLabel.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: DisplayUnitLabel property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/displayunitlabel/autoscalefont/
---
## DisplayUnitLabel.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public override bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(duLabelSrc.AutoScaleFont, duLabelDest.AutoScaleFont, info + ".AutoScaleFont");
public static void Property_AutoScaleFont(DisplayUnitLabel duLabelSrc, DisplayUnitLabel duLabelDest, string info)
        {
            if (AssertHelper.checkNull(duLabelSrc, duLabelDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(duLabelSrc.Text, duLabelDest.Text, info + ".Text");
            //=============compare patterns===============//
            LineTest.Property_AutoScaleFont(duLabelSrc.Border, duLabelDest.Border, info + ".Border");
            AreaTest.Property_AutoScaleFont(duLabelSrc.Area, duLabelDest.Area, info + ".Area");
            //=============compare font===================//
            FontTest.Property_AutoScaleFont(duLabelSrc.TextFont, duLabelDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(duLabelSrc.AutoScaleFont, duLabelDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(duLabelSrc.BackgroundMode, duLabelDest.BackgroundMode, info + ".BackgroundMode");
            //=============compare alignment=================//
            AssertHelper.AreEqual(duLabelSrc.TextHorizontalAlignment, duLabelDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
            AssertHelper.AreEqual(duLabelSrc.TextVerticalAlignment, duLabelDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
            AssertHelper.AreEqual(duLabelSrc.TextDirection, duLabelDest.TextDirection, info + ".TextDirection");
            AssertHelper.AreEqual(duLabelSrc.RotationAngle, duLabelDest.RotationAngle, info + ".RotationAngle");
            //=============compare other=================//
            AssertHelper.AreEqual(duLabelSrc.Height, duLabelDest.Height, info + ".Height");
            AssertHelper.AreEqual(duLabelSrc.Width, duLabelDest.Width, info + ".Width");

            AssertHelper.AreEqual(duLabelSrc.Shadow, duLabelDest.Shadow, info + ".Shadow");
            ShapePropertiesTest.Property_AutoScaleFont(duLabelSrc.ShapeProperties, duLabelDest.ShapeProperties, info + ".ShapeProperties");
            AssertHelper.AreEqual(duLabelSrc.IsAutomaticSize, duLabelDest.IsAutomaticSize, info + ".IsAutomaticSize");
        }
```

### See Also

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


