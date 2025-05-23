---
title: Series.GapWidth
second_title: Aspose.Cells for .NET API Reference
description: Series property. Returns or sets the space between bar or column clusters as a percentage of the bar or column width. The value of this property must be between 0 and 500
type: docs
url: /net/aspose.cells.charts/series/gapwidth/
---
## Series.GapWidth property

Returns or sets the space between bar or column clusters, as a percentage of the bar or column width. The value of this property must be between 0 and 500.

```csharp
public short GapWidth { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(33, workbook.Worksheets[0].Charts[0].NSeries[0].GapWidth);
public void Series_Property_GapWidth()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(ChartType.Funnel, workbook.Worksheets[0].Charts[0].Type);
    Assert.AreEqual(33, workbook.Worksheets[0].Charts[0].NSeries[0].GapWidth);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(33, workbook.Worksheets[0].Charts[0].NSeries[0].GapWidth);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


