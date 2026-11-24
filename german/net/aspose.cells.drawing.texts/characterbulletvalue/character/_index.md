---
title: "CharacterBulletValue.Character"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CharacterBulletValue-Eigenschaft. Gibt das Zeichen der Aufzählung zurück und setzt es"
type: docs
url: /de/net/aspose.cells.drawing.texts/characterbulletvalue/character/
---
## CharacterBulletValue.Character property

Liest und setzt das Zeichen der Aufzählung.

```csharp
public char Character { get; set; }
```

### Beispiele

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

### Siehe auch

* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


