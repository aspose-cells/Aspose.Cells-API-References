---
title: Chart.PlotBy
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets whether plot by row or column
type: docs
url: /net/aspose.cells.charts/chart/plotby/
---
## Chart.PlotBy property

Gets and sets whether plot by row or column.

```csharp
public PlotDataByType PlotBy { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.PlotBy, PlotDataByType.Column);
public void Chart_Property_PlotBy()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.PlotBy, PlotDataByType.Column);

}
```

### See Also

* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


