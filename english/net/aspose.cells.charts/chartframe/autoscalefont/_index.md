---
title: ChartFrame.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(titleSrc.AutoScaleFont, titleDest.AutoScaleFont, info + &amp;quot;.AutoScaleFont&amp;quot;);
public static void Property_AutoScaleFont(Title titleSrc, Title titleDest, string info)
        {
            if (AssertHelper.checkNull(titleSrc, titleDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(titleSrc.Text, titleDest.Text, info + &quot;.Text&quot;);
            Line lineSrc = titleSrc.Border;
            Line lineDest = titleDest.Border;
            LineTest.Property_AutoScaleFont(lineSrc, lineDest, info + &quot;.Border&quot;);
            Area areaSrc = titleSrc.Area;
            Area areaDest = titleDest.Area;
            AreaTest.Property_AutoScaleFont(areaSrc, areaDest, info + &quot;.Area&quot;);
            Font fontSrc = titleSrc.TextFont;
            Font fontDest = titleDest.TextFont;
            FontTest.Property_AutoScaleFont(fontSrc, fontDest, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(titleSrc.AutoScaleFont, titleDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(titleSrc.BackgroundMode, titleDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            AssertHelper.AreEqual(titleSrc.Shadow, titleDest.Shadow, info+&quot;.Shadow&quot;);
            AssertHelper.AreEqual(titleSrc.TextHorizontalAlignment, titleDest.TextHorizontalAlignment, info + &quot;.TextHorizontalAlignment&quot;);
            AssertHelper.AreEqual(titleSrc.TextVerticalAlignment, titleDest.TextVerticalAlignment, info + &quot;.TextVerticalAlignment&quot;);
            AssertHelper.AreEqual(titleSrc.TextDirection, titleDest.TextDirection, info + &quot;.TextDirection&quot;);
            AssertHelper.AreEqual(titleSrc.RotationAngle, titleDest.RotationAngle, info + &quot;.RotationAngle&quot;);            
            AssertHelper.AreEqual(titleSrc.Height, titleDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(titleSrc.Width, titleDest.Width, info + &quot;.Width&quot;);
            AssertHelper.AreEqual(titleSrc.X, titleDest.X, info + &quot;.X&quot;);
            AssertHelper.AreEqual(titleSrc.Y, titleDest.Y, info + &quot;.Y&quot;);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


