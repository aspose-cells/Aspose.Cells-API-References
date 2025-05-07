---
title: TextParagraphCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: TextParagraphCollection property. Gets the count of text paragraphs
type: docs
url: /net/aspose.cells.drawing.texts/textparagraphcollection/count/
---
## TextParagraphCollection.Count property

Gets the count of text paragraphs.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, ps.Count);
[Test]
        public void Property_Count()
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
            wb.Save(Constants.destPath + "CELLSJAVA41865.xlsx");
            wb = new Workbook(Constants.destPath + "CELLSJAVA41865.xlsx");
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

* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


