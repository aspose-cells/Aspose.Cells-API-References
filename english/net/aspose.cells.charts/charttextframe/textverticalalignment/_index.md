---
title: ChartTextFrame.TextVerticalAlignment
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets or sets the text vertical alignment of text
type: docs
url: /net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

Gets or sets the text vertical alignment of text.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(duLabelSrc.TextVerticalAlignment, duLabelDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
public static void ChartTextFrame_Property_TextVerticalAlignment(DisplayUnitLabel duLabelSrc, DisplayUnitLabel duLabelDest, string info)
        {
            if (AssertHelper.checkNull(duLabelSrc, duLabelDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(duLabelSrc.Text, duLabelDest.Text, info + ".Text");
            //=============compare patterns===============//
            LineTest.ChartTextFrame_Property_TextVerticalAlignment(duLabelSrc.Border, duLabelDest.Border, info + ".Border");
            AreaTest.ChartTextFrame_Property_TextVerticalAlignment(duLabelSrc.Area, duLabelDest.Area, info + ".Area");
            //=============compare font===================//
            FontTest.ChartTextFrame_Property_TextVerticalAlignment(duLabelSrc.TextFont, duLabelDest.TextFont, info + ".TextFont");
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
            ShapePropertiesTest.ChartTextFrame_Property_TextVerticalAlignment(duLabelSrc.ShapeProperties, duLabelDest.ShapeProperties, info + ".ShapeProperties");
            AssertHelper.AreEqual(duLabelSrc.IsAutomaticSize, duLabelDest.IsAutomaticSize, info + ".IsAutomaticSize");
        }
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


