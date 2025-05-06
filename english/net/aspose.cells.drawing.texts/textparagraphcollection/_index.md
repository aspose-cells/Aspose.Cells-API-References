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
// Called: TextParagraphCollection ps = shape.TextBody.TextParagraphs;
[Test]
        public void Type_TextParagraphCollection()
        {
            Workbook wb = new Workbook();

            Shape shape = wb.Worksheets[0].Shapes.AddTextBox(0, 0, 0, 0, 100, 300);
            shape.Text = &quot;STRAHINJA\nMISIC\nCAR&quot;;
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
            wb.Save(Constants.destPath + &quot;CELLSJAVA41865.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSJAVA41865.xlsx&quot;);
            shape = wb.Worksheets[0].Shapes[0];
            Assert.AreEqual(shape.Text, &quot;STRAHINJA\nMISIC\nCAR&quot;);
            line = 0;
            TextParagraphCollection ps = shape.TextBody.TextParagraphs;
            Assert.AreEqual(3, ps.Count);
            for (line = 0; line &lt; 3; line++)
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

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


