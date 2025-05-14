---
title: FontSettingCollection.GetParagraphEnumerator
second_title: Aspose.Cells for .NET API Reference
description: FontSettingCollection method. Gets the enumerator of the paragraphs
type: docs
url: /net/aspose.cells.drawing.texts/fontsettingcollection/getparagraphenumerator/
---
## FontSettingCollection.GetParagraphEnumerator method

Gets the enumerator of the paragraphs.

```csharp
public IEnumerator GetParagraphEnumerator()
```

### Examples

```csharp
// Called: for (IEnumerator ie = shape.TextBody.GetParagraphEnumerator(); ie.MoveNext(); )
public void FontSettingCollection_Method_GetParagraphEnumerator()
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

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


