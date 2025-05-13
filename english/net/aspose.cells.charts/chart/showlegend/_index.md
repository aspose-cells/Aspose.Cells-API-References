---
title: Chart.ShowLegend
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets or sets a value indicating whether the chart legend will be displayed. Default is true
type: docs
url: /net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Gets or sets a value indicating whether the chart legend will be displayed. Default is true.

```csharp
public bool ShowLegend { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.ShowLegend, true, "ShowLegend");
public void Chart_Property_ShowLegend()
{
    Workbook wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];
    int chartIndex = sheet.Charts.Add(ChartType.Waterfall, 10, 2, 20, 10);
    Chart chart = sheet.Charts[chartIndex];
    chart.NSeries.Add("{10,20,30,40}", true);
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    chart = wb.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.ShowLegend, true, "ShowLegend");
    chart.ShowLegend = false;
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    chart = wb.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.ShowLegend, false, "ShowLegend");
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


