---
title: Axis.MajorTickMark
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Represents the type of major tick mark for the specified axis
type: docs
url: /net/aspose.cells.charts/axis/majortickmark/
---
## Axis.MajorTickMark property

Represents the type of major tick mark for the specified axis.

```csharp
public TickMarkType MajorTickMark { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].Charts[0].ValueAxis.MajorTickMark, TickMarkType.Cross);
[Test]
        public void Property_MajorTickMark()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET46562.ods&quot;);
            Assert.IsTrue(workbook.Worksheets[1].Charts[0].CategoryAxis.MajorGridLines.IsVisible);
            Assert.AreEqual(workbook.Worksheets[1].Charts[0].ValueAxis.MajorTickMark, TickMarkType.Cross);
            workbook.Save(Constants.destPath + &quot;CELLSNET46562.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET46562.xlsx&quot;);
            Assert.IsTrue(workbook.Worksheets[1].Charts[0].CategoryAxis.MajorGridLines.IsVisible);
            Assert.AreEqual(workbook.Worksheets[1].Charts[0].ValueAxis.MajorTickMark, TickMarkType.Cross);
            Assert.AreEqual(&quot;=Tabellen!$C$20:$C$20&quot;, workbook.Worksheets[1].Charts[0].NSeries[0].Name);
        }
```

### See Also

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


