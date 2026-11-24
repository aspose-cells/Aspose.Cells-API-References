---
title: "Klasse Bullet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.Bullet-Klasse. Stellt die Aufzählungspunkte dar, die auf einen Absatz angewendet werden sollen."
type: docs
url: /de/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Stellt die Aufzählungspunkte dar, die auf einen Absatz angewendet werden sollen.

```csharp
public class Bullet
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Liest den Wert von bullet. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Liest und setzt den Namen der Schriftart. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Liest und setzt den Typ von bullet. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletDemo
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

            workbook.Save("TextsClassBulletDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


