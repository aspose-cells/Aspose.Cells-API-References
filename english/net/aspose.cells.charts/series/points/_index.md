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
// Called: Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.ShowCellRange, true);
public void Series_Property_Points()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.ShowCellRange, true);

}
```

### See Also

* class [ChartPointCollection](../../chartpointcollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


