---
title: "FontSettingCollection.TextParagraphs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSettingCollection-Eigenschaft. Gibt alle Absätze zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Liest alle Absätze.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextParagraphsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Greife auf den ersten Textabsatz zu
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Lege Zeilenabstandseigenschaften fest
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Lege Aufzählungseigenschaften fest
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


