---
title: ChartPointCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: ChartPointCollection method. Remove all setting of the chart points
type: docs
url: /net/aspose.cells.charts/chartpointcollection/clear/
---
## ChartPointCollection.Clear method

Remove all setting of the chart points.

```csharp
public void Clear()
```

### Examples

```csharp
// Called: chart.NSeries[0].Points.Clear();
[Test]
        public void Method_Clear()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestBubble_134989.xls&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].Name = &quot;=C1&quot;;
            chart.NSeries[0].XValues = &quot;B24&quot;;
            chart.NSeries[0].Values = &quot;B26&quot;;
            chart.NSeries[0].BubbleSizes = &quot;C2&quot;;

            chart.CategoryAxis.MinValue = 0;
            chart.CategoryAxis.MaxValue = 2;
            chart.CategoryAxis.MajorUnit = 1;
            chart.CategoryAxis.MinorUnit = 1;
            chart.NSeries.IsColorVaried = false;
            chart.NSeries[0].Points.Clear();

            workbook.Save(Constants.destPath + &quot;TestBubble_134989.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestBubble_134989.xls&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.MaxValue, 2);
        }
```

### See Also

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


