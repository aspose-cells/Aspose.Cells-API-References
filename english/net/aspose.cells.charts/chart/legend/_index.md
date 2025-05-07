---
title: Chart.Legend
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the chart legend
type: docs
url: /net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Gets the chart legend.

```csharp
public Legend Legend { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(LegendPositionType.Left, chart.Legend.Position, "chart.Legend.Position");
private void Property_Legend(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet5"];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(LegendPositionType.Left, chart.Legend.Position, "chart.Legend.Position");
        }
```

### See Also

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


