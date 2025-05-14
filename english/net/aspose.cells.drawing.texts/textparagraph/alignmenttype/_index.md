---
title: TextParagraph.AlignmentType
second_title: Aspose.Cells for .NET API Reference
description: TextParagraph property. Gets and sets the text horizontal alignment type of the paragraph
type: docs
url: /net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Gets and sets the text horizontal alignment type of the paragraph.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Examples

```csharp
// Called: p.AlignmentType = TextAlignmentType.Right;
public void TextParagraph_Property_AlignmentType()
{
    Workbook wb = new Workbook();

    Shape shape = wb.Worksheets[0].Shapes.AddTextBox(0, 0, 0, 0, 100, 300);
    shape.Text = "STRAHINJA\nMISIC\nCAR";
    int line = 0;
    for (IEnumerator ie = shape.TextBody.GetParagraphEnumerator(); ie.MoveNext(); )
    {
        TextParagraph p = (TextParagraph)ie.Current;
        switch (line)
        {
            case 0:
                p.AlignmentType = TextAlignmentType.Center;
                break;
            case 1:
                p.AlignmentType = TextAlignmentType.Left;
                break;
            case 2:
                p.AlignmentType = TextAlignmentType.Right;
                break;
        }
        line++;
    }
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    shape = wb.Worksheets[0].Shapes[0];
    Assert.AreEqual(shape.Text, "STRAHINJA\nMISIC\nCAR");
    line = 0;
    TextParagraphCollection ps = shape.TextBody.TextParagraphs;
    Assert.AreEqual(3, ps.Count);
    for (line = 0; line < 3; line++)
    {
        TextParagraph p = ps[line];
        switch (line)
        {
            case 0:
                Assert.AreEqual(p.AlignmentType, TextAlignmentType.Center);
                break;
            case 1:
                Assert.AreEqual(p.AlignmentType, TextAlignmentType.Left);
                break;
            case 2:
                Assert.AreEqual(p.AlignmentType, TextAlignmentType.Right);
                break;
        }
    }
}
```

### See Also

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


