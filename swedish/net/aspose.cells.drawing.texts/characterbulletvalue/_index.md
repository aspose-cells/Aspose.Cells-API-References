---
title: "Klass CharacterBulletValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.CharacterBulletValue-klass. Representerar teckenpunkten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Representerar teckenpunkten.

```csharp
public class CharacterBulletValue : BulletValue
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Hämtar och anger tecknet för punkten. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Hämtar typen av punkten. |

### Exempel

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

### Se även

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


