---
title: "Enum BulletType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.BulletType enum. Representerar typen av punkt"
type: docs
url: /sv/net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Representerar typen av punkt.

```csharp
public enum BulletType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen punkt. |
| Character | `1` | Teckenpunkt. |
| Picture | `2` | Bildpunkt. |
| AutoNumbered | `3` | Automatisk numrerad punkt. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en TextBox och ange text
            TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "Sample text with bullet type demonstration";

            // Skapa punktalternativ
            NoneBulletValue noneBullet = new NoneBulletValue();
            BulletType bulletType = noneBullet.Type;

            // Applicera punktinställningar på textparagrafer
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                paragraph.Bullet.Type = bulletType;
            }

            Console.WriteLine("Bullet Type applied: " + bulletType);
            workbook.Save("BulletTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


