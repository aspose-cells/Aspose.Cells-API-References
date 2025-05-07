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
// Called: AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + ".BackgroundMode");
public static void Property_BackgroundMode(LegendEntry legendentrySrc, LegendEntry legendentryDest, string info)
        {
            if (AssertHelper.checkNull(legendentrySrc, legendentryDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(legendentrySrc.IsDeleted, legendentryDest.IsDeleted, info + ".IsDeleted");
            FontTest.Property_BackgroundMode(legendentrySrc.Font, legendentryDest.Font, info + ".TextFont");
            AssertHelper.AreEqual(legendentrySrc.AutoScaleFont, legendentryDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + ".BackgroundMode");
           
        }
```

### See Also

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


