---
title: "Enum BulletType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Texts.BulletType. Rappresenta il tipo di pallino"
type: docs
url: /it/net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Rappresenta il tipo di punto elenco.

```csharp
public enum BulletType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun pallino. |
| Character | `1` | Pallino a carattere. |
| Picture | `2` | Pallino immagine. |
| AutoNumbered | `3` | Pallino numerato automatico. |

### Esempi

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

            // Crea una TextBox e imposta il testo
            TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "Sample text with bullet type demonstration";

            // Crea opzioni di elenco puntato
            NoneBulletValue noneBullet = new NoneBulletValue();
            BulletType bulletType = noneBullet.Type;

            // Applica le impostazioni di elenco puntato ai paragrafi di testo
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

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


