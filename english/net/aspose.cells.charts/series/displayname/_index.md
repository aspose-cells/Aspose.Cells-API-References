---
title: Series.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the seriess name that displays on the chart graph
type: docs
url: /net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Gets the series's name that displays on the chart graph.

```csharp
public string DisplayName { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;JPM US Equity&amp;quot;, chart.NSeries[0].DisplayName);
[Test]
        public void Property_DisplayName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;47619.xlsx&quot;);
            Chart chart = workbook.Worksheets[1].Charts[0];
            chart.SetChartDataRange(&quot;ChartCDSSpread!A1:E24&quot;, true);
            Assert.AreEqual(4, chart.NSeries.Count);
            if (string.IsNullOrEmpty(chart.NSeries[1].Name))
            {
                Assert.Fail(&quot;chart.NSeries[1].Name should not be empty&quot;);
            }

            workbook = new Workbook(Constants.sourcePath + &quot;47619.xlsx&quot;);
            chart = workbook.Worksheets[1].Charts[0];
            chart.SetChartDataRange(&quot;ChartCDSSpread!B1:E24&quot;, true);
            Assert.AreEqual(4, chart.NSeries.Count);
            if (!string.IsNullOrEmpty(chart.NSeries.CategoryData))
            {
                Assert.Fail(&quot;chart.NSeries.CategoryData should be empty&quot;);
            }
            Assert.AreEqual(&quot;JPM US Equity&quot;, chart.NSeries[0].DisplayName);

            workbook = new Workbook(Constants.sourcePath + &quot;47619.xlsx&quot;);
            chart = workbook.Worksheets[1].Charts[0];
            chart.SetChartDataRange(&quot;ChartCDSSpread!A2:E24&quot;, true);
            Assert.AreEqual(4, chart.NSeries.Count);
            if (string.IsNullOrEmpty(chart.NSeries.CategoryData))
            {
                Assert.Fail(&quot;chart.NSeries.CategoryData should not be empty&quot;);
            }
            if (!string.IsNullOrEmpty(chart.NSeries[0].Name))
            {
                Assert.Fail(&quot;chart.NSeries[1].Name should be empty&quot;);
            }
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


