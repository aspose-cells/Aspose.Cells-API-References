---
title: Series.TrendLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns all the trendlines of this series
type: docs
url: /net/aspose.cells.charts/series/trendlines/
---
## Series.TrendLines property

Returns all the trendlines of this series.

```csharp
public TrendlineCollection TrendLines { get; }
```

### Examples

```csharp
// Called: Trendline trendline = chart.NSeries[0].TrendLines[0];
private void Series_Property_TrendLines(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet5"];
            Chart chart = sheet.Charts[0];
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            AssertHelper.AreEqual(TrendlineType.Exponential, trendline.Type, "chart.NSeries[0].TrendLines[0].Type");
        }
```

### See Also

* class [TrendlineCollection](../../trendlinecollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


