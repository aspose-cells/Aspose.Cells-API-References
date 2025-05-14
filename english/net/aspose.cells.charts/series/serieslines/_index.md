---
title: Series.SeriesLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts
type: docs
url: /net/aspose.cells.charts/series/serieslines/
---
## Series.SeriesLines property

Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart. Applies only to stacked bar and stacked column charts.

```csharp
public Line SeriesLines { get; }
```

### Examples

```csharp
// Called: serie.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
public void Series_Property_SeriesLines()
{
    Workbook book = new Workbook();
    Worksheet sheet = book.Worksheets[0];
    int chartIndex = sheet.Charts.Add(ChartType.Scatter, 10, 2, 20, 10);
    Chart chart = sheet.Charts[chartIndex];
    int seriesIndex = chart.NSeries.Add("{10,20,30,40}", true);
    Series serie = chart.NSeries[seriesIndex];
    serie.Smooth = true;
    serie.Type = ChartType.Line;
    serie.SeriesLines.Color = Color.Red;
    serie.SeriesLines.Weight = Aspose.Cells.Drawing.WeightType.SingleLine;
    book.Save(Constants.destPath + "example.xlsx");
    book.Dispose();
    book = new Workbook(Constants.destPath + "example.xlsx");
    chart = book.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].Type, ChartType.Line, "ChartType");
    Assert.AreEqual(chart.NSeries[0].Marker.MarkerStyle, ChartMarkerType.None, "ChartType");

}
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


