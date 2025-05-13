---
title: TrendlineCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TrendlineCollection property. Gets a Trendline object by its index
type: docs
url: /net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Gets a [`Trendline`](../../trendline/) object by its index.

```csharp
public Trendline this[int index] { get; }
```

### Examples

```csharp
// Called: Trendline trendline = chart.NSeries[0].TrendLines[0];
private void TrendlineCollection_Property_Item(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            AssertHelper.AreEqual(TrendlineType.Linear, trendline.Type, "chart.NSeries[0].TrendLines[0].Type");
        }
```

### See Also

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


