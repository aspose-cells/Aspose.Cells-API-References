---
title: ChartPoint.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Returns a DataLabels object that represents the data label associated with this chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Returns a `DataLabels` object that represents the data label associated with this chart point.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;800&amp;quot;, chart.NSeries[1].Points[2].DataLabels.Text);
[Test]
        public void Property_DataLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/ChartAPI/TimChartORama-source.xlsx&quot;);
            Chart chart = workbook.Worksheets[&quot;HELLO CHARTS&quot;].Charts[0];
            chart.Calculate(new ChartCalculateOptions() { UpdateAllPoints = true });
            Assert.AreEqual(&quot;100&quot;, chart.NSeries[0].Points[0].DataLabels.Text);
            Assert.AreEqual(&quot;200&quot;, chart.NSeries[0].Points[1].DataLabels.Text);
            Assert.AreEqual(&quot;300&quot;, chart.NSeries[0].Points[2].DataLabels.Text);
            Assert.AreEqual(&quot;Custom Data Label 2&quot;, chart.NSeries[0].Points[3].DataLabels.Text);

            Assert.AreEqual(&quot;400&quot;, chart.NSeries[1].Points[0].DataLabels.Text);
            Assert.AreEqual(&quot;Custom Data Label 1&quot;, chart.NSeries[1].Points[1].DataLabels.Text);
            Assert.AreEqual(&quot;800&quot;, chart.NSeries[1].Points[2].DataLabels.Text);
            Assert.AreEqual(&quot;1000&quot;, chart.NSeries[1].Points[3].DataLabels.Text);

            Assert.AreEqual(&quot;100&quot;, chart.NSeries[2].Points[0].DataLabels.Text);
            Assert.AreEqual(&quot;500&quot;, chart.NSeries[2].Points[1].DataLabels.Text);
            Assert.AreEqual(&quot;900&quot;, chart.NSeries[2].Points[2].DataLabels.Text);
            Assert.AreEqual(&quot;1200&quot;, chart.NSeries[2].Points[3].DataLabels.Text);
        }
```

### See Also

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


