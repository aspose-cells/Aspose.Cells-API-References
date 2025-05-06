---
title: Series.LayoutProperties
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the properties of layout
type: docs
url: /net/aspose.cells.charts/series/layoutproperties/
---
## Series.LayoutProperties property

Represents the properties of layout.

```csharp
public SeriesLayoutProperties LayoutProperties { get; }
```

### Examples

```csharp
// Called: series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
[Test]
        public void Property_LayoutProperties()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;MapChart_001.xlsx&quot;);
            Aspose.Cells.Charts.ChartCollection chars = workbook.Worksheets[1].Charts;
            chars.Add(ChartType.Map, 6, 3, 26, 12);
            Chart chart = chars[0];
            chart.NSeries.Add(&quot;B8:B108&quot;, true);
            Series series = chart.NSeries[0];
            series.Name = &quot;=B7&quot;;
            series.XValues = &quot;A8:A108&quot;;
            series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
            series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
            series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

            workbook.Save(Constants.destPath + &quot;MapChart_001.xlsx&quot;);
        }
```

### See Also

* class [SeriesLayoutProperties](../../serieslayoutproperties/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


