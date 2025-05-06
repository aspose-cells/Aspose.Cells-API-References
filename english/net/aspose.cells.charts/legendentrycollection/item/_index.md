---
title: LegendEntryCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: LegendEntryCollection property. Gets the LegendEntry element at the specified index
type: docs
url: /net/aspose.cells.charts/legendentrycollection/item/
---
## LegendEntryCollection indexer

Gets the [`LegendEntry`](../../legendentry/) element at the specified index.

```csharp
public LegendEntry this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: entries[0].IsDeleted = true;
[Test]
        public void Property_Int32_()
        {
            int nSeries = 2;
            var workbook = new Workbook();
            int index = workbook.Worksheets.Add();
            var worksheet = workbook.Worksheets[index];
            index = worksheet.Charts.Add(ChartType.Scatter, 0, 0, 5, 2);
            var chart = worksheet.Charts[index];

            chart.ChartObject.HeightInch = 4;
            chart.ChartObject.WidthInch = 6;

            string[] yvalues = { &quot;{1,3,5,7,9}&quot;, &quot;{2,4,6,8,10}&quot; };

            for (int i = 0; i &lt; nSeries; ++i)
            {
                index = chart.NSeries.Add(&quot;A1&quot;, false);
                var series = chart.NSeries[index];
                series.XValues = &quot;{1,2,3,4,5}&quot;;
                series.Values = yvalues[i];
                index = series.TrendLines.Add(TrendlineType.Linear);
            }

            var entries = chart.Legend.LegendEntries;
            entries[0].IsDeleted = true;

            //  workbook.Save(@&quot;Test3.pdf&quot;);
            workbook.Save(Constants.destPath + @&quot;CELLSNET47508.xlsx&quot;);
        }
```

### See Also

* class [LegendEntry](../../legendentry/)
* class [LegendEntryCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


