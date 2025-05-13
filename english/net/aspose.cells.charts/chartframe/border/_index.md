---
title: ChartFrame.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets the border
type: docs
url: /net/aspose.cells.charts/chartframe/border/
---
## ChartFrame.Border property

Gets the [`border`](../../../aspose.cells.drawing/line/).

```csharp
public virtual Line Border { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(WeightType.MediumLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
private void ChartFrame_Property_Border(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(WeightType.MediumLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


