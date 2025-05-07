---
title: Bullet.BulletValue
second_title: Aspose.Cells for .NET API Reference
description: Bullet property. Gets the value of bullet
type: docs
url: /net/aspose.cells.drawing.texts/bullet/bulletvalue/
---
## Bullet.BulletValue property

Gets the value of bullet.

```csharp
public BulletValue BulletValue { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(((CharacterBulletValue)bullet.BulletValue).Character, 'v');
[Test]
        public void Property_BulletValue()
        {
            Workbook workbook = new Workbook();
            // Get the first worksheet in the book.
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a new textbox to the collection.
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);

            // Get the textbox object.
            Aspose.Cells.Drawing.TextBox textbox0 = worksheet.TextBoxes[textboxIndex];
            // Fill the text.
            textbox0.Text = "   Sample text";

            textbox0.TextBody.TextParagraphs[0].LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Percentage;
            textbox0.TextBody.TextParagraphs[0].LineSpace = 3000;

            Bullet bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';

            bullet.FontName = "Arial";
            workbook.Save(Constants.destPath + "CellsNet47291.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet47291.xlsx");
            Shape shape = workbook.Worksheets[0].Shapes[0];
            bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
            Assert.AreEqual(bullet.Type, BulletType.Character);
            Assert.AreEqual(((CharacterBulletValue)bullet.BulletValue).Character, 'v');
            Assert.AreEqual(bullet.FontName, "Arial");
        }
```

### See Also

* class [BulletValue](../../bulletvalue/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


