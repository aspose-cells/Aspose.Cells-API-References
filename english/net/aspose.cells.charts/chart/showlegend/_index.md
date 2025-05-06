---
title: Chart.ShowLegend
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets a value indicating whether the chart legend will be displayed. Default is true
type: docs
url: /net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

```csharp
public bool ShowLegend { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ShowLegend, true, &amp;quot;ShowLegend&amp;quot;);
[Test]
        public void Property_ShowLegend()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            int chartIndex = sheet.Charts.Add(ChartType.Waterfall, 10, 2, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;{10,20,30,40}&quot;, true);
            wb.Save(Constants.destPath + &quot;CELLSNET50197.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET50197.xlsx&quot;);
            chart = wb.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.ShowLegend, true, &quot;ShowLegend&quot;);
            chart.ShowLegend = false;
            wb.Save(Constants.destPath + &quot;CELLSNET50197_2.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET50197_2.xlsx&quot;);
            chart = wb.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.ShowLegend, false, &quot;ShowLegend&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


