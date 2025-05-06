---
title: SeriesCollection.SwapSeries
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection method. Directly changes the orders of the two series
type: docs
url: /net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

Directly changes the orders of the two series.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |

### Examples

```csharp
// Called: sc.SwapSeries(2, 0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/ChartAPI/excel_input.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            SeriesCollection sc = chart.NSeries;
            Assert.AreEqual(3, sc.Count);
            Assert.AreEqual(&quot;Net Units&quot;, sc[0].Name);
            Assert.AreEqual(&quot;Return Units&quot;, sc[1].Name);
            Assert.AreEqual(&quot;Gross Units&quot;, sc[2].Name);
            sc.SwapSeries(0, 1);
            Assert.AreEqual(&quot;Return Units&quot;, sc[0].Name);
            Assert.AreEqual(&quot;Net Units&quot;, sc[1].Name);
            Assert.AreEqual(&quot;Gross Units&quot;, sc[2].Name);
            sc.SwapSeries(2, 0);
            Assert.AreEqual(&quot;Gross Units&quot;, sc[0].Name);
            Assert.AreEqual(&quot;Net Units&quot;, sc[1].Name);
            Assert.AreEqual(&quot;Return Units&quot;, sc[2].Name);
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


