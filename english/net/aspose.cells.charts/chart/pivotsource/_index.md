---
title: Chart.PivotSource
second_title: Aspose.Cells for .NET API Reference
description: Chart property. The source is the data of the pivotTable. If PivotSource is not empty the chart is PivotChart
type: docs
url: /net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

The source is the data of the pivotTable. If PivotSource is not empty ,the chart is PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Remarks

If the pivot table "PivotTable1" in the Worksheet "Sheet1" in the file "Book1.xls". The pivotSource could be "[Book1.xls]Sheet1!PivotTable1" if the chart and the PivotTable is not in the same workbook. If you set this property ,the previous data source setting will be lost.

### Examples

```csharp
// Called: chart.PivotSource = &amp;quot;CasPivot!PivotTable2&amp;quot;;
public static void Property_PivotSource(Worksheet worksheet2)
        {
            int indexChart = worksheet2.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet2.Charts[indexChart];
            chart.PivotSource = &quot;CasPivot!PivotTable2&quot;;
            chart.HidePivotFieldButtons = false;
            chart.RefreshPivotData();
            chart.PlotArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.None;
            chart.PlotArea.Border.IsVisible = false;
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


