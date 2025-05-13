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
// Called: ChartPoint p = chart.NSeries[0].Points[7];
private void ChartPointCollection_Property_Item(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[7];
            ChartPoint p = chart.NSeries[0].Points[7];
            AssertHelper.AreEqual(FillPattern.LightHorizontal, p.Area.FillFormat.Pattern, "chart.NSeries[7].Area.FillFormat.Pattern");
        }
```

### See Also

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


