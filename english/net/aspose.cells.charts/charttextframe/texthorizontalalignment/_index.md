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
// Called: AssertHelper.AreEqual(titleSrc.TextHorizontalAlignment, titleDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
public static void ChartTextFrame_Property_TextHorizontalAlignment(Title titleSrc, Title titleDest, string info)
        {
            if (AssertHelper.checkNull(titleSrc, titleDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(titleSrc.Text, titleDest.Text, info + ".Text");
            Line lineSrc = titleSrc.Border;
            Line lineDest = titleDest.Border;
            LineTest.ChartTextFrame_Property_TextHorizontalAlignment(lineSrc, lineDest, info + ".Border");
            Area areaSrc = titleSrc.Area;
            Area areaDest = titleDest.Area;
            AreaTest.ChartTextFrame_Property_TextHorizontalAlignment(areaSrc, areaDest, info + ".Area");
            Font fontSrc = titleSrc.TextFont;
            Font fontDest = titleDest.TextFont;
            FontTest.ChartTextFrame_Property_TextHorizontalAlignment(fontSrc, fontDest, info + ".TextFont");
            AssertHelper.AreEqual(titleSrc.AutoScaleFont, titleDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(titleSrc.BackgroundMode, titleDest.BackgroundMode, info + ".BackgroundMode");
            AssertHelper.AreEqual(titleSrc.Shadow, titleDest.Shadow, info+".Shadow");
            AssertHelper.AreEqual(titleSrc.TextHorizontalAlignment, titleDest.TextHorizontalAlignment, info + ".TextHorizontalAlignment");
            AssertHelper.AreEqual(titleSrc.TextVerticalAlignment, titleDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
            AssertHelper.AreEqual(titleSrc.TextDirection, titleDest.TextDirection, info + ".TextDirection");
            AssertHelper.AreEqual(titleSrc.RotationAngle, titleDest.RotationAngle, info + ".RotationAngle");            
            AssertHelper.AreEqual(titleSrc.Height, titleDest.Height, info + ".Height");
            AssertHelper.AreEqual(titleSrc.Width, titleDest.Width, info + ".Width");
            AssertHelper.AreEqual(titleSrc.X, titleDest.X, info + ".X");
            AssertHelper.AreEqual(titleSrc.Y, titleDest.Y, info + ".Y");
        }
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


