---
title: "BulletValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "BulletValue-Eigenschaft. Gibt den Typ des Aufzählungswerts zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Ermittelt den Typ des Aufzählungszeichenwerts.

```csharp
public abstract BulletType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle ein Textfeld und rufe seine Textabsätze ab
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Erstelle einen Zeichen‑BulletValue (der von BulletValue erbt)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Den Wert der Type-Eigenschaft anzeigen
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Erstelle einen Bild‑BulletValue, um einen anderen Typ anzuzeigen
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Speichere die Arbeitsmappe
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


