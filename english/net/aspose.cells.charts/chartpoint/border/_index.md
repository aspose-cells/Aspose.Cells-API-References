---
title: ChartPoint.Border
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  border
type: docs
url: /net/aspose.cells.charts/chartpoint/border/
---
## ChartPoint.Border property

Gets the [` border`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(p.Border.Style, Aspose.Cells.Drawing.LineType.Solid);
[Test]
        public void Property_Border()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet30785.xls&quot;);
            Chart c = wb.Worksheets[0].Charts[0];
            Series s = c.NSeries[0];
            ChartPoint p = s.Points[1];
            p.Border.Color = Color.Red; //it works
            p.Border.Style = Aspose.Cells.Drawing.LineType.Solid; //it does not work
            Assert.AreEqual(p.Border.Style, Aspose.Cells.Drawing.LineType.Solid);

            wb.Save(Constants.destPath + &quot;CellsNet30785.xls&quot;);

        }
```

### See Also

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


