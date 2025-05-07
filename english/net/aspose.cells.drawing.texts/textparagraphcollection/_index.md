---
title: Class TextParagraphCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.TextParagraphCollection class. Represents all text paragraph
type: docs
url: /net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Represents all text paragraph.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Gets the count of text paragraphs. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Gets the [`TextParagraph`](../textparagraph/) object at specific index. |

## Methods

| Name | Description |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Gets the enumerator of the paragraphs. |

### Examples

```csharp
// Called: TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
[Test]
        public void Type_TextParagraphCollection()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            Shape shape = workbook.Worksheets[0].Shapes[0];
            shape.Text = "abc\nefg";
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4;
            workbook.Save(Constants.destPath + "CELLSNET43167.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET43167.xlsx");
            p = workbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            Assert.AreEqual(p.SpaceBeforeSizeType, LineSpaceSizeType.Points);
            Assert.AreEqual(p.SpaceAfterSizeType, LineSpaceSizeType.Points);
            Assert.AreEqual(p.LineSpaceSizeType, LineSpaceSizeType.Points);
            Assert.AreEqual(2, p.LineSpace);
            Assert.AreEqual(3, p.SpaceAfter);
            Assert.AreEqual(4, p.SpaceBefore);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


