---
title: Cell.EmbeddedImage
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets and sets the embeddedn image in the cell
type: docs
url: /net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Gets and sets the embeddedn image in the cell.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(a.Worksheets[0].Cells[&amp;quot;B6&amp;quot;].EmbeddedImage != null);
[Test]
        public void Property_EmbeddedImage()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET55331_Workbook.xlsx&quot;);
            Workbook a = new Workbook();
            a.Worksheets[0].Cells.CopyRows(wb.Worksheets[0].Cells,5,5,1);
            Assert.IsTrue(a.Worksheets[0].Cells[&quot;B6&quot;].EmbeddedImage != null);
            a = new Workbook();
            a.Worksheets[0].Cells.CopyColumns(wb.Worksheets[0].Cells, 1, 1, 1);
            Assert.IsTrue(a.Worksheets[0].Cells[&quot;B6&quot;].EmbeddedImage != null);
            a.Save(Constants.destPath + &quot;CELLSNET55331_RowColumn.xlsx&quot;);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


