---
title: Chart.HidePivotFieldButtons
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Indicates whether hide the pivot chart field buttons only when the chart is PivotChart
type: docs
url: /net/aspose.cells.charts/chart/hidepivotfieldbuttons/
---
## Chart.HidePivotFieldButtons property

Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.

```csharp
public bool HidePivotFieldButtons { get; set; }
```

### Examples

```csharp
// Called: chart.HidePivotFieldButtons = false;
public static void Chart_Property_HidePivotFieldButtons(Worksheet worksheet2)
        {
            int indexChart = worksheet2.Charts.Add(ChartType.Column3DClustered, 9, 6, 24, 14);
            Chart chart = worksheet2.Charts[indexChart];
            chart.PivotSource = "CasPivot!PivotTable2";
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


