---
title: TickLabels.Font
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Returns a Font object that represents the font of the specified TickLabels object
type: docs
url: /net/aspose.cells.charts/ticklabels/font/
---
## TickLabels.Font property

Returns a `Font` object that represents the font of the specified TickLabels object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: var fontName = workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-48386.xlsx&quot;);
            var fontName = workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
            Assert.AreEqual(&quot;Generis Sans Com&quot;, fontName, &quot;TickLabels.Font.Name&quot;);
            var newWorkbook = new Workbook();
            newWorkbook.Copy(workbook);
            var fontNameCopied = newWorkbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
            Assert.AreEqual(&quot;Generis Sans Com&quot;, fontNameCopied, &quot;TickLabels.Font.Name&quot;);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


