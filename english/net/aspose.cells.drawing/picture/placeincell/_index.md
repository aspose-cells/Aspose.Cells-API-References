---
title: Picture.PlaceInCell
second_title: Aspose.Cells for .NET API Reference
description: Picture method. Place this picture in the cell
type: docs
url: /net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

Place this picture in the cell

```csharp
public void PlaceInCell()
```

### Examples

```csharp
// Called: w.Worksheets[0].Pictures[0].PlaceInCell();
[Test]
        public void Method_PlaceInCell()
        {
            Workbook w = new Workbook(Constants.sourcePath + &quot;CellsNet56062.xlsx&quot;);
            w.Worksheets[0].Pictures[0].PlaceInCell();
            Assert.IsTrue(w.Worksheets[0].Cells[&quot;B2&quot;].EmbeddedImage != null);
            w.Save(Constants.destPath + &quot;CellsNet56062.xlsx&quot;);
        }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


