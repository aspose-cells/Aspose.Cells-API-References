---
title: Bullet.Type
second_title: Aspose.Cells for .NET API Reference
description: Bullet property. Gets and sets the type of bullet
type: docs
url: /net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Gets and sets the type of bullet.

```csharp
public BulletType Type { get; set; }
```

### Examples

```csharp
// Called: bullet.Type = BulletType.Character;
[Test]
        public void Property_Type()
        {
            Workbook workbook = new Workbook();
            // Get the first worksheet in the book.
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a new textbox to the collection.
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);

            // Get the textbox object.
            Aspose.Cells.Drawing.TextBox textbox0 = worksheet.TextBoxes[textboxIndex];
            // Fill the text.
            textbox0.Text = &quot;   Sample text&quot;;

            textbox0.TextBody.TextParagraphs[0].LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Percentage;
            textbox0.TextBody.TextParagraphs[0].LineSpace = 3000;

            Bullet bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = &apos;v&apos;;

            bullet.FontName = &quot;Arial&quot;;
            workbook.Save(Constants.destPath + &quot;CellsNet47291.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet47291.xlsx&quot;);
            Shape shape = workbook.Worksheets[0].Shapes[0];
            bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
            Assert.AreEqual(bullet.Type, BulletType.Character);
            Assert.AreEqual(((CharacterBulletValue)bullet.BulletValue).Character, &apos;v&apos;);
            Assert.AreEqual(bullet.FontName, &quot;Arial&quot;);
        }
```

### See Also

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


