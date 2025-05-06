---
title: ChartFrame.Shadow
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. True if the frame has a shadow
type: docs
url: /net/aspose.cells.charts/chartframe/shadow/
---
## ChartFrame.Shadow property

True if the frame has a shadow.

```csharp
public bool Shadow { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + &amp;quot;.Shadow&amp;quot;);
public static void Property_Shadow(ChartFrame cframeSrc, ChartFrame cframeDest, string info)
        {
            if (AssertHelper.checkNull(cframeSrc, cframeDest, info))
            {
                return;
            }
            LineTest.Property_Shadow(cframeSrc.Border, cframeDest.Border, info + &quot;.Border&quot;);
            AreaTest.Property_Shadow(cframeSrc.Area, cframeDest.Area, info + &quot;.Area&quot;);
            AssertHelper.AreEqual(cframeSrc.AutoScaleFont, cframeDest.AutoScaleFont, info+&quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(cframeSrc.BackgroundMode, cframeDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
            AssertHelper.AreEqual(cframeSrc.Height, cframeDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(cframeSrc.Shadow, cframeDest.Shadow, info + &quot;.Shadow&quot;);
            FontTest.Property_Shadow(cframeSrc.Font, cframeDest.Font, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(cframeSrc.Width, cframeDest.Width, info + &quot;.Width&quot;);
            AssertHelper.AreEqual(cframeSrc.X, cframeDest.X, info + &quot;.X&quot;);
            AssertHelper.AreEqual(cframeSrc.Y, cframeDest.Y, info + &quot;.Y&quot;);

            AssertHelper.AreEqual(cframeSrc.IsAutomaticSize, cframeDest.IsAutomaticSize, info + &quot;.IsAutomaticSize&quot;);
            ShapePropertiesTest.Property_Shadow(cframeSrc.ShapeProperties, cframeDest.ShapeProperties, info + &quot;.ShapeProperties&quot;);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


