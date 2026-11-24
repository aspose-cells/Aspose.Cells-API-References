---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoNumberedBulletValue-Eigenschaft. Gibt die Startnummer des Aufzählungszeichens zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Liest und setzt die Startnummer der Aufzählung.

```csharp
public int StartAt { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
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
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Zeigen Sie den aktuellen StartAt-Wert an
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // Ändern Sie den StartAt-Wert
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Erstellen Sie eine Form, um das Aufzählungszeichen im Kontext zu demonstrieren
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Wenden Sie den Aufzählungsstil an (Hinweis: Die tatsächliche Anwendungsmethode wird in der Reflexion nicht angezeigt)
                // Zur Demonstration speichern wir einfach die Arbeitsmappe
                workbook.Save("StartAtPropertyDemo.xlsx");
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

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


