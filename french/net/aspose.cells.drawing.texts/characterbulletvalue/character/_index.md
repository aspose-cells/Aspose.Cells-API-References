---
title: "CharacterBulletValue.Character"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CharacterBulletValue. Obtient et définit le caractère de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/characterbulletvalue/character/
---
## CharacterBulletValue.Character property

Obtient et définit le caractère de la puce.

```csharp
public char Character { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class CharacterBulletValuePropertyCharacterDemo
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

            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


