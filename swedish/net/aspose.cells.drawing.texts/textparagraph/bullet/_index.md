---
title: "TextParagraph.Bullet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar punkten"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

Hämtar punkttecknet.

```csharp
public Bullet Bullet { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyBulletDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Ange text och konfigurera stycke
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // Konfigurera punkt för det första stycket
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Spara arbetsboken
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### Se även

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


