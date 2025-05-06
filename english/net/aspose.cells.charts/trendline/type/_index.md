---
title: Trendline.Type
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Returns the trendline type
type: docs
url: /net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Returns the trendline type.

```csharp
public TrendlineType Type { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TrendlineType.Exponential, trendline.Type, &amp;quot;chart.NSeries[0].TrendLines[0].Type&amp;quot;);
private void Property_Type(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            AssertHelper.AreEqual(TrendlineType.Exponential, trendline.Type, &quot;chart.NSeries[0].TrendLines[0].Type&quot;);
        }
```

### See Also

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


