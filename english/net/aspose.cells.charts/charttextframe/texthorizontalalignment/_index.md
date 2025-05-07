---
title: ChartTextFrame.TextHorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets the text horizontal alignment
type: docs
url: /net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Gets and sets the text horizontal alignment.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(duLabelSrc.TextHorizontalAlignment, duLabelDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
public static void Property_TextHorizontalAlignment(DisplayUnitLabel duLabelSrc, DisplayUnitLabel duLabelDest, string info)
        {
            if (AssertHelper.checkNull(duLabelSrc, duLabelDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(duLabelSrc.Text, duLabelDest.Text, info + ".Text");
            //=============compare patterns===============//
            LineTest.Property_TextHorizontalAlignment(duLabelSrc.Border, duLabelDest.Border, info + ".Border");
            AreaTest.Property_TextHorizontalAlignment(duLabelSrc.Area, duLabelDest.Area, info + ".Area");
            //=============compare font===================//
            FontTest.Property_TextHorizontalAlignment(duLabelSrc.TextFont, duLabelDest.TextFont, info + ".TextFont");
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
            ShapePropertiesTest.Property_TextHorizontalAlignment(duLabelSrc.ShapeProperties, duLabelDest.ShapeProperties, info + ".ShapeProperties");
            AssertHelper.AreEqual(duLabelSrc.IsAutomaticSize, duLabelDest.IsAutomaticSize, info + ".IsAutomaticSize");
        }
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


