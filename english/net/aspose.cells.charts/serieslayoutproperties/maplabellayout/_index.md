---
title: SeriesLayoutProperties.MapLabelLayout
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Gets and sets the layout of map labels
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/maplabellayout/
---
## SeriesLayoutProperties.MapLabelLayout property

Gets and sets the layout of map labels.

```csharp
public MapChartLabelLayout MapLabelLayout { get; set; }
```

### Examples

```csharp
// Called: series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
public void SeriesLayoutProperties_Property_MapLabelLayout()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.Charts.ChartCollection chars = workbook.Worksheets[1].Charts;
    chars.Add(ChartType.Map, 6, 3, 26, 12);
    Chart chart = chars[0];
    chart.NSeries.Add("B8:B108", true);
    Series series = chart.NSeries[0];
    series.Name = "=B7";
    series.XValues = "A8:A108";
    series.LayoutProperties.MapChartProjectionType = MapChartProjectionType.Mercator;
    series.LayoutProperties.MapLabelLayout = MapChartLabelLayout.ShowAll;
    series.LayoutProperties.MapChartRegionType = MapChartRegionType.DataOnly;

    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [MapChartLabelLayout](../../mapchartlabellayout/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


