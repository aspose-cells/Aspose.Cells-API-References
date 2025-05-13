---
title: Chart.PlotArea
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts plot area which includes axis tick labels
type: docs
url: /net/aspose.cells.charts/chart/plotarea/
---
## Chart.PlotArea property

Gets the chart's plot area which includes axis tick labels.

```csharp
public PlotArea PlotArea { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.PlotArea.Area.FillFormat.FillType, Aspose.Cells.Drawing.FillType.Gradient);
public void Chart_Property_PlotArea()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.PlotArea.Area.FillFormat.FillType, Aspose.Cells.Drawing.FillType.Gradient);
}
```

### See Also

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


