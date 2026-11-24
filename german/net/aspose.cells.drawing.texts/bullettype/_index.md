---
title: "Enum BulletType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.BulletType enum. Stellt den Typ des Aufzählungszeichens dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Stellt den Typ des Aufzählungszeichens dar.

```csharp
public enum BulletType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Kein Aufzählungszeichen. |
| Character | `1` | Zeichen‑Aufzählungszeichen. |
| Picture | `2` | Bild‑Aufzählungszeichen. |
| AutoNumbered | `3` | Automatisches nummeriertes Aufzählungszeichen. |

### Beispiele

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

            // Erstellen Sie ein TextBox und setzen Sie den Text
            TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "Sample text with bullet type demonstration";

            // Erstellen Sie Aufzählungsoptionen
            NoneBulletValue noneBullet = new NoneBulletValue();
            BulletType bulletType = noneBullet.Type;

            // Wenden Sie Aufzählungseinstellungen auf Textabsätze an
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

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


