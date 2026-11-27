---
title: "FontSettingCollection.TextParagraphs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontSettingCollection-egenskap. Hämtar alla stycken"
type: docs
url: /sv/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Hämtar alla stycken.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i arbetsbladet
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Få åtkomst till det första textstycket
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Ange radavståndsegenskaper
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Ange punktlistans egenskaper
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Spara arbetsboken
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


