---
title: Series.BubbleSizes
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets the bubble sizes values of the chart series
type: docs
url: /net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Gets or sets the bubble sizes values of the chart series.

```csharp
public string BubbleSizes { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].BubbleSizes = "C2";
public void Series_Property_BubbleSizes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].Name = "=C1";
    chart.NSeries[0].XValues = "B24";
    chart.NSeries[0].Values = "B26";
    chart.NSeries[0].BubbleSizes = "C2";

    chart.CategoryAxis.MinValue = 0;
    chart.CategoryAxis.MaxValue = 2;
    chart.CategoryAxis.MajorUnit = 1;
    chart.CategoryAxis.MinorUnit = 1;
    chart.NSeries.IsColorVaried = false;
    chart.NSeries[0].Points.Clear();

    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.CategoryAxis.MaxValue, 2);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


