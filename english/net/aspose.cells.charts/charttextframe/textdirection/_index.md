---
title: ChartTextFrame.TextDirection
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Represents text reading order
type: docs
url: /net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

Represents text reading order.

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use ChartTextFrame.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(duLabelSrc.TextDirection, duLabelDest.TextDirection, info + &amp;quot;.TextDirection&amp;quot;);
public static void Property_TextDirection(DisplayUnitLabel duLabelSrc, DisplayUnitLabel duLabelDest, string info)
        {
            if (AssertHelper.checkNull(duLabelSrc, duLabelDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(duLabelSrc.Text, duLabelDest.Text, info + &quot;.Text&quot;);
            //=============compare patterns===============//
            LineTest.Property_TextDirection(duLabelSrc.Border, duLabelDest.Border, info + &quot;.Border&quot;);
            AreaTest.Property_TextDirection(duLabelSrc.Area, duLabelDest.Area, info + &quot;.Area&quot;);
            //=============compare font===================//
            FontTest.Property_TextDirection(duLabelSrc.TextFont, duLabelDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(duLabelSrc.AutoScaleFont, duLabelDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(duLabelSrc.BackgroundMode, duLabelDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            //=============compare alignment=================//
            AssertHelper.AreEqual(duLabelSrc.TextHorizontalAlignment, duLabelDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
            AssertHelper.AreEqual(duLabelSrc.TextVerticalAlignment, duLabelDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
            AssertHelper.AreEqual(duLabelSrc.TextDirection, duLabelDest.TextDirection, info + &quot;.TextDirection&quot;);
            AssertHelper.AreEqual(duLabelSrc.RotationAngle, duLabelDest.RotationAngle, info + &quot;.RotationAngle&quot;);
            //=============compare other=================//
            AssertHelper.AreEqual(duLabelSrc.Height, duLabelDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(duLabelSrc.Width, duLabelDest.Width, info + &quot;.Width&quot;);

            AssertHelper.AreEqual(duLabelSrc.Shadow, duLabelDest.Shadow, info + &quot;.Shadow&quot;);
            ShapePropertiesTest.Property_TextDirection(duLabelSrc.ShapeProperties, duLabelDest.ShapeProperties, info + &quot;.ShapeProperties&quot;);
            AssertHelper.AreEqual(duLabelSrc.IsAutomaticSize, duLabelDest.IsAutomaticSize, info + &quot;.IsAutomaticSize&quot;);
        }
```

### See Also

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


