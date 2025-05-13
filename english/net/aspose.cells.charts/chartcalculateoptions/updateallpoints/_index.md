---
title: ChartCalculateOptions.UpdateAllPoints
second_title: Aspose.Cells for .NET API Reference
description: ChartCalculateOptions property. Whether update all data points when performing the chart calculation. Default False. When you want to get the value for each data point in the chart specifically set it to true. If this parameter is set to True the new data points may be generated when chart is calculated. This could make the Excel file larger
type: docs
url: /net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Examples

```csharp
// Called: chart.Calculate(new ChartCalculateOptions() { UpdateAllPoints = true });
public void ChartCalculateOptions_Property_UpdateAllPoints()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/TimChartORama-source.xlsx");
    Chart chart = workbook.Worksheets["HELLO CHARTS"].Charts[0];
    chart.Calculate(new ChartCalculateOptions() { UpdateAllPoints = true });
    Assert.AreEqual("100", chart.NSeries[0].Points[0].DataLabels.Text);
    Assert.AreEqual("200", chart.NSeries[0].Points[1].DataLabels.Text);
    Assert.AreEqual("300", chart.NSeries[0].Points[2].DataLabels.Text);
    Assert.AreEqual("Custom Data Label 2", chart.NSeries[0].Points[3].DataLabels.Text);

    Assert.AreEqual("400", chart.NSeries[1].Points[0].DataLabels.Text);
    Assert.AreEqual("Custom Data Label 1", chart.NSeries[1].Points[1].DataLabels.Text);
    Assert.AreEqual("800", chart.NSeries[1].Points[2].DataLabels.Text);
    Assert.AreEqual("1000", chart.NSeries[1].Points[3].DataLabels.Text);

    Assert.AreEqual("100", chart.NSeries[2].Points[0].DataLabels.Text);
    Assert.AreEqual("500", chart.NSeries[2].Points[1].DataLabels.Text);
    Assert.AreEqual("900", chart.NSeries[2].Points[2].DataLabels.Text);
    Assert.AreEqual("1200", chart.NSeries[2].Points[3].DataLabels.Text);
}
```

### See Also

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


