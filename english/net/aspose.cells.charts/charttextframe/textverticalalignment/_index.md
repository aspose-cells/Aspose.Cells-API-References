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
// Called: AssertHelper.AreEqual(titleSrc.TextVerticalAlignment, titleDest.TextVerticalAlignment, info + ".TextVerticalAlignment");
public static void Property_TextVerticalAlignment(Title titleSrc, Title titleDest, string info)
        {
            if (AssertHelper.checkNull(titleSrc, titleDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(titleSrc.Text, titleDest.Text, info + ".Text");
            Line lineSrc = titleSrc.Border;
            Line lineDest = titleDest.Border;
            LineTest.Property_TextVerticalAlignment(lineSrc, lineDest, info + ".Border");
            Area areaSrc = titleSrc.Area;
            Area areaDest = titleDest.Area;
            AreaTest.Property_TextVerticalAlignment(areaSrc, areaDest, info + ".Area");
            Font fontSrc = titleSrc.TextFont;
            Font fontDest = titleDest.TextFont;
            FontTest.Property_TextVerticalAlignment(fontSrc, fontDest, info + ".TextFont");
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


