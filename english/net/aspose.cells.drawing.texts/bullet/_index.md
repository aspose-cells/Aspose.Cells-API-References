---
title: Class Bullet
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.Bullet class. Represents the bullet points should be applied to a paragraph
type: docs
url: /net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Represents the bullet points should be applied to a paragraph.

```csharp
public class Bullet
```

## Properties

| Name | Description |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Gets the value of bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Get and sets the name of the font. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Gets and sets the type of bullet. |

### Examples

```csharp
// Called: Bullet bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
public void Texts_Type_Bullet()
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
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Shape shape = workbook.Worksheets[0].Shapes[0];
    bullet = textbox0.TextBody.TextParagraphs[0].Bullet;
    Assert.AreEqual(bullet.Type, BulletType.Character);
    Assert.AreEqual(((CharacterBulletValue)bullet.BulletValue).Character, 'v');
    Assert.AreEqual(bullet.FontName, "Arial");
}
```

### See Also

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


