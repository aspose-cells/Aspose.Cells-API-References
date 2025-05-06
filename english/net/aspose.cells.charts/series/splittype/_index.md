---
title: Series.SplitType
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart
type: docs
url: /net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of pie chart.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
[Test]
        public void Property_SplitType()
        {
            Workbook workbook = new Workbook();
            workbook = TestPiePie.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].SplitType = ChartSplitType.PercentValue;

            checkChartSplitType_PercentValue(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkChartSplitType_PercentValue(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkChartSplitType_PercentValue(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


