---
title: Chart.ChartArea
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the chart area in the worksheet
type: docs
url: /net/aspose.cells.charts/chart/chartarea/
---
## Chart.ChartArea property

Gets the chart area in the worksheet.

```csharp
public ChartArea ChartArea { get; }
```

### Examples

```csharp
// Called: ChartArea chartarea = chart.ChartArea;
private void Chart_Property_ChartArea(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(WeightType.SingleLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
        }
```

### See Also

* class [ChartArea](../../chartarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


