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
// Called: chart.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
[Test]
        public void Property_PlotEmptyCellsType()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            checkPlotEmptyCellsType_Zero(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkPlotEmptyCellsType_Zero(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkPlotEmptyCellsType_Zero(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


