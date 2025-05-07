---
title: ShapeTextAlignment.NumberOfColumns
second_title: Aspose.Cells for .NET API Reference
description: ShapeTextAlignment property. Gets and sets the number of columns of text in the bounding rectangle
type: docs
url: /net/aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/
---
## ShapeTextAlignment.NumberOfColumns property

Gets and sets the number of columns of text in the bounding rectangle.

```csharp
public int NumberOfColumns { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, workbook.Worksheets[0].Shapes[0].TextBody.TextAlignment.NumberOfColumns);
[Test]
        public void Property_NumberOfColumns()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet51574.xlsx");
            workbook.Save(Constants.destPath + "CellsNet51574.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet51574.xlsx");
            Assert.AreEqual(2, workbook.Worksheets[0].Shapes[0].TextBody.TextAlignment.NumberOfColumns);
        }
```

### See Also

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


