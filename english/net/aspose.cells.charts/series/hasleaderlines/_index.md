---
title: Series.HasLeaderLines
second_title: Aspose.Cells for .NET API Reference
description: Series property. True if the series has leader lines
type: docs
url: /net/aspose.cells.charts/series/hasleaderlines/
---
## Series.HasLeaderLines property

True if the series has leader lines.

```csharp
public bool HasLeaderLines { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].HasLeaderLines, true);
[Test]
        public void Property_HasLeaderLines()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet42909.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].HasLeaderLines, true);
            workbook.Save(Constants.destPath + "CellsNet42909.xlsx");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].HasLeaderLines, true);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


