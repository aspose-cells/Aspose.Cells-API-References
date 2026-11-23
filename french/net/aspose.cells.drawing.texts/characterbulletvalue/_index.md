---
title: "Classe CharacterBulletValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.CharacterBulletValue. Représente la puce de caractère"
type: docs
url: /fr/net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Représente la puce de caractère.

```csharp
public class CharacterBulletValue : BulletValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Obtient et définit le caractère de la puce. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Obtient le type de la puce. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassCharacterBulletValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("CharacterBulletValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


