---
title: Series.Smooth
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts
type: docs
url: /net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```csharp
public bool Smooth { get; set; }
```

### Examples

```csharp
// Called: serie.Smooth = true;
[Test]
        public void Property_Smooth()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 10, 2, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add(&quot;{10,20,30,40}&quot;, true);
            Series serie = chart.NSeries[seriesIndex];
            serie.Smooth = true;
            serie.Type = ChartType.Line;
            serie.SeriesLines.Color = Color.Red;
            serie.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
            book.Save(Constants.destPath + &quot;CELLSNET50087.xlsx&quot;);
            book.Dispose();
            book = new Workbook(Constants.destPath + &quot;CELLSNET50087.xlsx&quot;);
            chart = book.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Type, ChartType.Line, &quot;ChartType&quot;);
            Assert.AreEqual(chart.NSeries[0].Marker.MarkerStyle, ChartMarkerType.None, &quot;ChartType&quot;);

        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


