---
title: Series.Points
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the collection of points in a series in a chart
type: docs
url: /net/aspose.cells.charts/series/points/
---
## Series.Points property

Gets the collection of points in a series in a chart.

```csharp
public ChartPointCollection Points { get; }
```

### Remarks

When the chart is Pie of Pie or Bar of Pie, the last point is other point in first pie plot.

### Examples

```csharp
// Called: ChartPoint p = chart.NSeries[0].Points[1];
private void Property_Points(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet6"];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[1];
            ChartPoint p = chart.NSeries[0].Points[1];
            AssertHelper.AreEqual(TextureType.Walnut, p.Area.FillFormat.Texture, "chart.NSeries[1].Area.FillFormat.Texture");
        }
```

### See Also

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


