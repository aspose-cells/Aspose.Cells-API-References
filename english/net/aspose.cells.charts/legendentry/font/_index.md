---
title: LegendEntry.Font
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets a Font object of the specified ChartFrame object
type: docs
url: /net/aspose.cells.charts/legendentry/font/
---
## LegendEntry.Font property

Gets a `Font` object of the specified ChartFrame object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: FontTest.equals(legendentrySrc.Font, legendentryDest.Font, info + &amp;quot;.TextFont&amp;quot;);
public static void Property_Font(LegendEntry legendentrySrc, LegendEntry legendentryDest, string info)
        {
            if (AssertHelper.checkNull(legendentrySrc, legendentryDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(legendentrySrc.IsDeleted, legendentryDest.IsDeleted, info + &quot;.IsDeleted&quot;);
            FontTest.Property_Font(legendentrySrc.Font, legendentryDest.Font, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(legendentrySrc.AutoScaleFont, legendentryDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + &quot;.BackgroundMode&quot;);
           
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


