---
title: Series.IsAutoSplit
second_title: Aspose.Cells for .NET API Reference
description: Series property. Indicates whether the threshold value is automatic
type: docs
url: /net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

Indicates whether the threshold value is automatic.

```csharp
public bool IsAutoSplit { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(chart.NSeries[0].IsAutoSplit);
public void Series_Property_IsAutoSplit()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "piepiechart_1.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.IsFalse(chart.NSeries[0].IsAutoSplit);
    Assert.AreEqual(3, chart.NSeries[0].SplitValue);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


