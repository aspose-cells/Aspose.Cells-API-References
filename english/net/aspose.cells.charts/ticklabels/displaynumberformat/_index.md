---
title: TickLabels.DisplayNumberFormat
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Gets and sets the display number format of tick labels
type: docs
url: /net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Gets and sets the display number format of tick labels.

```csharp
public string DisplayNumberFormat { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;m/d/yyyy&amp;quot;, workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.DisplayNumberFormat);
[Test]
        public void Property_DisplayNumberFormat()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + @&quot;CellsNet47447.xlsx&quot;);
            Assert.AreEqual(&quot;m/d/yyyy&quot;, workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.DisplayNumberFormat);
            Assert.AreEqual(&quot;General&quot;,workbook.Worksheets[0].Charts[0].ValueAxis.TickLabels.DisplayNumberFormat);

        }
```

### See Also

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


