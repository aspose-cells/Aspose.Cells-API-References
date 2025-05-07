---
title: LegendEntry.IsDeleted
second_title: Aspose.Cells for .NET API Reference
description: LegendEntry property. Gets and sets whether the legend entry is deleted
type: docs
url: /net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Gets and sets whether the legend entry is deleted.

```csharp
public bool IsDeleted { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendentrySrc.IsDeleted, legendentryDest.IsDeleted, info + ".IsDeleted");
public static void Property_IsDeleted(LegendEntry legendentrySrc, LegendEntry legendentryDest, string info)
        {
            if (AssertHelper.checkNull(legendentrySrc, legendentryDest, info))
            {
                return;
            }
            AssertHelper.AreEqual(legendentrySrc.IsDeleted, legendentryDest.IsDeleted, info + ".IsDeleted");
            FontTest.Property_IsDeleted(legendentrySrc.Font, legendentryDest.Font, info + ".TextFont");
            AssertHelper.AreEqual(legendentrySrc.AutoScaleFont, legendentryDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(legendentrySrc.BackgroundMode, legendentryDest.BackgroundMode, info + ".BackgroundMode");
           
        }
```

### See Also

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


