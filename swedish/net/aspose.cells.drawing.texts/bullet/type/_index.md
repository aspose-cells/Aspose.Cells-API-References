---
title: "Bullet.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Bullet-egenskap. Hämtar och anger typen av bullet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Hämtar och anger typen av bullet.

```csharp
public BulletType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Konfigurera bullet-egenskaper
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Spara arbetsboken
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


