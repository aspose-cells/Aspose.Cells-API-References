---
title: SeriesCollection.CategoryData
second_title: Aspose.Cells for .NET API Reference
description: SeriesCollection property. Gets or sets the range of category Axis values. It can be a range of cells such as d1e10 or a sequence of values such as26810
type: docs
url: /net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Gets or sets the range of category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Examples

```csharp
// Called: testAreEqual(&amp;quot;=Sheet1!$C$5:$C$21&amp;quot;, chart.NSeries.CategoryData, caseName);
private void Property_CategoryData(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            testAreEqual(&quot;=Sheet1!$D$3:$D$19&quot;, chart.NSeries[0].Values, caseName);
            testAreEqual(&quot;=Sheet1!$C$5:$C$21&quot;, chart.NSeries.CategoryData, caseName);
        }
```

### See Also

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


