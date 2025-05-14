---
title: Series.IsColorVaried
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents if the color of points is varied. The chart must contain only one series
type: docs
url: /net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Represents if the color of points is varied. The chart must contain only one series.

```csharp
public bool IsColorVaried { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].IsColorVaried, true);
public void Series_Property_IsColorVaried()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[1].Charts[0];
    Assert.AreEqual(chart.NSeries[0].IsColorVaried, true);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    chart = workbook.Worksheets[1].Charts[0];
    Assert.AreEqual(chart.NSeries[0].IsColorVaried, true);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


