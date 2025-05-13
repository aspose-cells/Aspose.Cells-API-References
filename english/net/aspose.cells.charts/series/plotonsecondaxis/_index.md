---
title: Series.PlotOnSecondAxis
second_title: Aspose.Cells for .NET API Reference
description: Series property. Indicates if this series is plotted on second value axis
type: docs
url: /net/aspose.cells.charts/series/plotonsecondaxis/
---
## Series.PlotOnSecondAxis property

Indicates if this series is plotted on second value axis.

```csharp
public bool PlotOnSecondAxis { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].PlotOnSecondAxis, true);
public void Series_Property_PlotOnSecondAxis()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets.AddCopy(workbook.Worksheets[0].Name);
    Chart chart = workbook.Worksheets[1].Charts[0];
    Assert.AreEqual(chart.NSeries[0].PlotOnSecondAxis, true);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


