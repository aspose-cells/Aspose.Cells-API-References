---
title: Series.SplitValue
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart
type: docs
url: /net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Returns or sets a value that shall be used to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```csharp
public double SplitValue { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].SplitValue = 10;
public void Series_Property_SplitValue()
{
    Workbook workbook = new Workbook();
    workbook = TestPiePie.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].SplitType = ChartSplitType.Custom;
    chart.NSeries[0].SplitValue = 10;

    checkChartSplitType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkChartSplitType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkChartSplitType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


