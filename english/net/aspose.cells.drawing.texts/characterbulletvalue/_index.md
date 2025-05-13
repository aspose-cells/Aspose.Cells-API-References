---
title: Class CharacterBulletValue
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.Texts.CharacterBulletValue class. Represents the character bullet
type: docs
url: /net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Represents the character bullet.

```csharp
public class CharacterBulletValue : BulletValue
```

## Constructors

| Name | Description |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Gets and sets character of the bullet. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Gets the type of the bullet. |

### Examples

```csharp
// Called: ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
public void Texts_Type_CharacterBulletValue()
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

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


