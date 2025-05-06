---
title: Chart.NSeries
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets a SeriesCollection collection representing the data series in the chart
type: docs
url: /net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series in the chart.

```csharp
public SeriesCollection NSeries { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(DataLabelsSeparatorType.Auto, chart.NSeries[0].DataLabels.SeparatorType, &amp;quot;chart.NSeries[0].DataLabels.Separator&amp;quot;);
private void Property_NSeries(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet1&quot;];
            Chart chart = sheet.Charts[0];
            AssertHelper.AreEqual(DataLabelsSeparatorType.Auto, chart.NSeries[0].DataLabels.SeparatorType, &quot;chart.NSeries[0].DataLabels.Separator&quot;);
        }
```

### See Also

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


