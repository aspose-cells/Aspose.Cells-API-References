---
title: Chart.SetChartDataRange
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Specifies data range for a chart
type: docs
url: /net/aspose.cells.charts/chart/setchartdatarange/
---
## Chart.SetChartDataRange method

Specifies data range for a chart.

```csharp
public void SetChartDataRange(string area, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

### Examples

```csharp
// Called: chart.SetChartDataRange("A1:G12", true);
public void Chart_Method_SetChartDataRange()
{
    var wb = new Workbook(Constants.sourcePath + "example.xlsx");
    var chart = wb.Worksheets[0].Charts[1];
    chart.SetChartDataRange("A1:G12", true);
    Assert.AreEqual(chart.NSeries[0].Name, "=Sheet1!$C$1:$C$2");
    Assert.AreEqual("=Sheet1!$A$3:$B$12", chart.NSeries.CategoryData);
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


