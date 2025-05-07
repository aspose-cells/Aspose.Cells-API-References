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
// Called: Assert.IsFalse(chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
[Test]
        public void Property_PlotArea()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "user file(ChartDataLabels).xls");
            Chart chart = workbook.Worksheets["Motivation impact"].Charts[0];
            Assert.IsFalse(chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
        }
```

### See Also

* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


