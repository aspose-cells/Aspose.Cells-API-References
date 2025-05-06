---
title: Chart.SetChartDataRange
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Specifies data range for a chart
type: docs
url: /net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Specifies data range for a chart.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### Examples

```csharp
// Called: chart.SetChartDataRange(&amp;quot;A1:G12&amp;quot;, true);
[Test]
        public void Method_Boolean_()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;CELLSNET48067.xlsx&quot;);
            var chart = wb.Worksheets[0].Charts[1];
            chart.SetChartDataRange(&quot;A1:G12&quot;, true);
            Assert.AreEqual(chart.NSeries.Count, 5);

            string outputFile = Constants.destPath + &quot;CELLSNET48067.xlsx&quot;;
            wb.Save(outputFile);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


