---
title: "Bullet.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Bullet. Ottiene e imposta il tipo di bullet"
type: docs
url: /it/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Ottiene e imposta il tipo di bullet.

```csharp
public BulletType Type { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Configura le proprietà del bullet
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Salva la cartella di lavoro
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


