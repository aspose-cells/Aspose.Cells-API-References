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
[Test]
        public void Property_GapWidth()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET46899.xlsx&quot;);
            Assert.AreEqual(ChartType.Funnel, workbook.Worksheets[0].Charts[0].Type);
            Assert.AreEqual(33, workbook.Worksheets[0].Charts[0].NSeries[0].GapWidth);
            workbook.Save(Constants.destPath + &quot;CELLSNET46899.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET46899.xlsx&quot;);
            Assert.AreEqual(33, workbook.Worksheets[0].Charts[0].NSeries[0].GapWidth);
            workbook.Save(Constants.destPath + &quot;CELLSNET46899.xlsx&quot;);
        }
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


