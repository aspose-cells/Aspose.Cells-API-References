---
title: Series.Border
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents border of Series object
type: docs
url: /net/aspose.cells.charts/series/border/
---
## Series.Border property

Represents border of Series object.

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(WeightType.HairLine, aseries.Border.Weight, "chart.NSeries[0].Line.Weight");
private void Series_Property_Border(Workbook workbook)
        {
            Chart chart = workbook.Worksheets[0].Charts[0];
            Series aseries = chart.NSeries[0];
            AssertHelper.AreEqual(WeightType.HairLine, aseries.Border.Weight, "chart.NSeries[0].Line.Weight");
        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


