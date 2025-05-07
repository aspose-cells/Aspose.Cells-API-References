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
// Called: AssertHelper.AreEqual(ChartSplitType.PercentValue, chart.NSeries[0].SplitType, "chart.NSeries[0].SplitType");
private void Property_SplitType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet3"];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(ChartSplitType.PercentValue, chart.NSeries[0].SplitType, "chart.NSeries[0].SplitType");
        }
```

### See Also

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


