---
title: Chart.PlotEmptyCellsType
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets how to plot the empty cells
type: docs
url: /net/aspose.cells.charts/chart/plotemptycellstype/
---
## Chart.PlotEmptyCellsType property

Gets and sets how to plot the empty cells.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(PlotEmptyCellsType.Zero, chart.PlotEmptyCellsType, "chart.PlotEmptyCellsType");
private void Chart_Property_PlotEmptyCellsType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(PlotEmptyCellsType.Zero, chart.PlotEmptyCellsType, "chart.PlotEmptyCellsType");
        }
```

### See Also

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


