---
title: Series.IsVerticalValues
second_title: Aspose.Cells for .NET API Reference
description: Series property. Indicates whether the data source is vertical
type: docs
url: /net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

Indicates whether the data source is vertical.

```csharp
public bool IsVerticalValues { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(charts[0].NSeries[0].IsVerticalValues, true);
[Test]
        public void Property_IsVerticalValues()
        {
            Workbook workbook = new Workbook();
            ChartCollection charts = workbook.Worksheets[0].Charts;
            charts.Add(ChartType.Column, 0, 0, 10, 10);
            charts[0].NSeries.Add(&quot;A1:B10&quot;, true);
            Assert.AreEqual(charts[0].NSeries[0].IsVerticalValues, true);

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


