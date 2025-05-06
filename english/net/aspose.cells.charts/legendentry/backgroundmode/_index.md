---
title: LegendEntry.BackgroundMode
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets and sets the display mode of the background
type: docs
url: /net/aspose.cells.charts/legendentry/backgroundmode/
---
## LegendEntry.BackgroundMode property

Gets and sets the display mode of the background

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + &amp;quot;.BackgroundMode&amp;quot;);
public static void Property_BackgroundMode(LegendEntry legendentrySrc, LegendEntry legendentryDest, string info)
        {
            if (AssertHelper.checkNull(legendentrySrc, legendentryDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(legendentrySrc.IsDeleted, legendentryDest.IsDeleted, info + &quot;.IsDeleted&quot;);
            FontTest.Property_BackgroundMode(legendentrySrc.Font, legendentryDest.Font, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(legendentrySrc.AutoScaleFont, legendentryDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
           
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


