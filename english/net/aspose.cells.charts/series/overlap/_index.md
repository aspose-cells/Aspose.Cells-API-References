---
title: Series.Overlap
second_title: Aspose.Cells for .NET API Reference
description: Series property. Specifies how bars and columns are positioned. Can be a value between  100 and 100. Applies only to 2D bar and 2D column charts
type: docs
url: /net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Specifies how bars and columns are positioned. Can be a value between – 100 and 100. Applies only to 2-D bar and 2-D column charts.

```csharp
public short Overlap { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].Overlap, -40);
[Test]
        public void Property_Overlap()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cellsnet43091.ods&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;grafici&quot;];
            Chart chart = sheet.Charts[0];
            Assert.AreEqual(chart.ShowLegend, true);
            Assert.AreEqual(chart.CategoryAxis.TickLabelPosition, TickLabelPositionType.NextToAxis);
            chart = sheet.Charts[&quot;Chart 3&quot;];
            Assert.AreEqual(chart.NSeries[0].Overlap, -40);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


