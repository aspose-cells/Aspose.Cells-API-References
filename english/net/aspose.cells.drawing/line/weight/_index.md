---
title: Line.Weight
second_title: Aspose.Cells for .NET API Reference
description: Line property. Gets or sets the WeightType of the line
type: docs
url: /net/aspose.cells.drawing/line/weight/
---
## Line.Weight property

Gets or sets the [`WeightType`](../../weighttype/) of the line.

```csharp
public WeightType Weight { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(WeightType.SingleLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
private void Property_Weight(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(WeightType.SingleLine, chartarea.Border.Weight, "chart.chartarea.Border.Weight");
        }
```

### See Also

* enum [WeightType](../../weighttype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


