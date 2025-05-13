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
// Called: ChartPoint p = chart.NSeries[0].Points[10];
private void SeriesCollection_Property_Item(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            Chart chart = sheet.Charts[0];
            //Series aseries = chart.NSeries[10];
            ChartPoint p = chart.NSeries[0].Points[10];
            AssertHelper.AreEqual(FillPattern.DarkVertical, p.Area.FillFormat.Pattern, "chart.NSeries[10].Area.FillFormat.Pattern");
        }
```

### See Also

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


