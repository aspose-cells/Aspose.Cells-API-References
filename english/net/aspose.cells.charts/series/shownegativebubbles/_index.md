---
title: Series.ShowNegativeBubbles
second_title: Aspose.Cells for .NET API Reference
description: Series property. True if negative bubbles are shown for the chart group. Valid only for bubble charts
type: docs
url: /net/aspose.cells.charts/series/shownegativebubbles/
---
## Series.ShowNegativeBubbles property

True if negative bubbles are shown for the chart group. Valid only for bubble charts.

```csharp
public bool ShowNegativeBubbles { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].ShowNegativeBubbles, false);
public void Series_Property_ShowNegativeBubbles()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].ShowNegativeBubbles, false);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].ShowNegativeBubbles, false);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


