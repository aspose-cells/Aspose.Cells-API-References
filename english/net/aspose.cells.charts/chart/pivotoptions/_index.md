---
title: Chart.PivotOptions
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Specifies the pivot controls that appear on the chart
type: docs
url: /net/aspose.cells.charts/chart/pivotoptions/
---
## Chart.PivotOptions property

Specifies the pivot controls that appear on the chart

```csharp
public PivotOptions PivotOptions { get; }
```

### Examples

```csharp
// Called: PivotOptions options = workbook.Worksheets[0].Charts[1].PivotOptions;
[Test]
        public void Property_PivotOptions()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet43845.xlsm&quot;);
            PivotOptions options = workbook.Worksheets[0].Charts[1].PivotOptions;
            Assert.IsFalse(options.DropZoneCategories);
            Assert.IsFalse(options.DropZoneData);
            Assert.IsFalse(options.DropZoneSeries);
        }
```

### See Also

* class [PivotOptions](../../pivotoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


