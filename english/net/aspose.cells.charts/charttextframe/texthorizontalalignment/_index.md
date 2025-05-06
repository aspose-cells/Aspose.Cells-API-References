---
title: ChartTextFrame.TextHorizontalAlignment
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets the text horizontal alignment
type: docs
url: /net/aspose.cells.charts/charttextframe/texthorizontalalignment/
---
## ChartTextFrame.TextHorizontalAlignment property

Gets and sets the text horizontal alignment.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(TextAlignmentType.Left, chart.Title.TextHorizontalAlignment);
[Test]
        public void Property_TextHorizontalAlignment()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-53258.xlsx&quot;);

            workbook.Save(Constants.destPath + &quot;CellsNet53258.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet53258.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(TextAlignmentType.Left, chart.Title.TextHorizontalAlignment);
        }
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


