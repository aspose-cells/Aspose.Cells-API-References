---
title: Series.Smooth
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts
type: docs
url: /net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Represents curve smoothing. True if curve smoothing is turned on for the line chart or scatter chart. Applies only to line and scatter connected by lines charts.

```csharp
public bool Smooth { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue( chart1.NSeries[0].Smooth);
public void Series_Property_Smooth()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet ws = workbook.Worksheets["Sheet1"];
    Chart chart1 = ws.Charts[1];
    Chart chart2 = ws.Charts[2];
   Assert.IsTrue( chart1.NSeries[0].Smooth);
    Assert.IsFalse( chart2.NSeries[0].Smooth);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


