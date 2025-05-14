---
title: TextParagraph.LineSpace
second_title: Aspose.Cells for .NET API Reference
description: TextParagraph property. Gets and sets the amount of vertical white space that will be used within a paragraph
type: docs
url: /net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Gets and sets the amount of vertical white space that will be used within a paragraph.

```csharp
public double LineSpace { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, p.LineSpace);
public void TextParagraph_Property_LineSpace()
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
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
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

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


