---
title: "Bullet.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Bullet-Eigenschaft. Liest und setzt den Typ des Aufzählungszeichens"
type: docs
url: /de/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Liest und setzt den Typ von bullet.

```csharp
public BulletType Type { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Textfeld hinzufügen
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Bullet-Eigenschaften konfigurieren
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Speichere die Arbeitsmappe
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


