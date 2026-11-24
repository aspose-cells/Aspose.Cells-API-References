---
title: "Klasse AutoNumberedBulletValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue Klasse. Stellt eine automatisch nummerierte Aufzählung dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/autonumberedbulletvalue/
---
## AutoNumberedBulletValue class

Stellt eine automatisch nummerierte Aufzählung dar.

```csharp
public class AutoNumberedBulletValue : BulletValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Stellt das Schema der automatischen Nummerierung dar. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Liest und setzt die Startnummer der Aufzählung. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Liest den Typ der Aufzählung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassAutoNumberedBulletValueDemo
    {
        public static void Run()
        {
            try
            {
                // Erstelle ein neues Arbeitsbuch
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Eine AutoNumberedBulletValue-Instanz erstellen
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
                    StartAt = 1
                };

                // Aufzählungseigenschaften anzeigen
                Console.WriteLine($"Bullet Type: {bullet.Type}");
                Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
                Console.WriteLine($"Starting Number: {bullet.StartAt}");

                // Eigenschaften ändern
                bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
                bullet.StartAt = 5;

                // Speichere die Arbeitsmappe
                workbook.Save("TextsClassAutoNumberedBulletValueDemo.xlsx");
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

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


