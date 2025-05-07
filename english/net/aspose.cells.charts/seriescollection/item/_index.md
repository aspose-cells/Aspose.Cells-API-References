---
title: SeriesCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Gets the Series element at the specified index
type: docs
url: /net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Gets the [`Series`](../../series/) element at the specified index.

```csharp
public Series this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Series aseries = chart.NSeries[1];
private void Property_Int32_(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            Series aseries = chart.NSeries[1];
            AssertHelper.AreEqual(WeightType.SingleLine, aseries.Border.Weight, "chart.NSeries[0].Line.Weight");
        }
```

### See Also

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


