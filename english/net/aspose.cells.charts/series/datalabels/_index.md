---
title: Series.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the DataLabels object for the specified ASeries
type: docs
url: /net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Represents the DataLabels object for the specified ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels.ShowPercentage);
[Test]
        public void Property_DataLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;TestDoughnut_001.xls&quot;);
            ChartCollection charts = workbook.Worksheets[0].Charts;
            charts.Add(ChartType.Doughnut, 5, 5, 15, 10);
            charts[0].NSeries.Add(&quot;A1:B3&quot;, true);
            charts[0].NSeries[0].DataLabels.ShowPercentage = true;
            workbook.Save(Constants.destPath + &quot;TestDoughnut_001.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestDoughnut_001.xls&quot;);
            Console.WriteLine(workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels.ShowPercentage);
        }
```

### See Also

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


