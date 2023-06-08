---
title: Chart.IsChartDataChanged
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Detects if a charts data source has changed
type: docs
url: /net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

Detects if a chart's data source has changed.

```csharp
public bool IsChartDataChanged()
```

### Return Value

Returns true if the chart has changed otherwise returns false

### Remarks

The method detects the changes in the chart's data source before rendering the chart to image format. At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded. Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


