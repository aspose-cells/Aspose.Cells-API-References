---
title: ChartPointCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ChartPointCollection property. Gets the ChartPoint element at the specified index in the series
type: docs
url: /net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Gets the [`ChartPoint`](../../chartpoint/) element at the specified index in the series.

```csharp
public ChartPoint this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index of chart point in the series. |

### Return Value

The ChartPoint object.

### Examples

```csharp
// Called: ChartPoint p = chart.NSeries[0].Points[5];
private void Property_Int32_(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet2&quot;];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[5];
            ChartPoint p = chart.NSeries[0].Points[5];
            AssertHelper.AreEqual(FillPattern.WideUpwardDiagonal, p.Area.FillFormat.Pattern, &quot;chart.NSeries[5].Area.FillFormat.Pattern&quot;);
        }
```

### See Also

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


