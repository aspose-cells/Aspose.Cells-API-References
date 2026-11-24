---
title: "Klasse CharacterBulletValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.CharacterBulletValue Klasse. Stellt die Zeichenaufzählung dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Stellt die Zeichen‑Aufzählung dar.

```csharp
public class CharacterBulletValue : BulletValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Liest und setzt das Zeichen der Aufzählung. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Liest den Typ der Aufzählung. |

### Beispiele

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

### Siehe auch

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


