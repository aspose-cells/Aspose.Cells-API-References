---
title: ChartFrame.Font
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets a Font object of the specified ChartFrame object
type: docs
url: /net/aspose.cells.charts/chartframe/font/
---
## ChartFrame.Font property

Gets a `Font` object of the specified ChartFrame object.

```csharp
public virtual Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(10, chart.Legend.Font.Size);
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet53283.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(10, chart.Legend.Font.Size);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


