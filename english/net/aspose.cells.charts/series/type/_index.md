---
title: Series.Type
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets a data series type
type: docs
url: /net/aspose.cells.charts/series/type/
---
## Series.Type property

Gets or sets a data series' type.

```csharp
public ChartType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ChartType.ColumnStacked, ser.Type);
public void Series_Property_Type()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    foreach (Series ser in chart.NSeries)
    {
        Assert.AreEqual(ChartType.ColumnStacked, ser.Type);
    }
}
```

### See Also

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


