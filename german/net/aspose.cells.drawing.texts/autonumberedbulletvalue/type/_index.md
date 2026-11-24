---
title: "AutoNumberedBulletValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoNumberedBulletValue-Eigenschaft. Gibt den Typ des Aufzählungszeichens zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Liest den Typ der Aufzählung.

```csharp
public override BulletType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Form, um Text mit Aufzählungszeichen hinzuzufügen
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Erstellen Sie einen automatisch nummerierten Aufzählungswert
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Da wir BulletValue nicht direkt setzen können, müssen wir einen anderen Weg finden
            // um den Aufzählungsstil anzuwenden. Dies könnte die Verwendung der Textformatierung der Form erfordern
            // oder andere verfügbare Methoden in der API.
            // Zur Demonstration zeigen wir einfach den Aufzählungstyp an
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Fügen Sie Text zum Absatz über den Textkörper der Form hinzu
            shape.TextBody.Text = "First Item";

            // Fügen Sie einen weiteren Absatz mit einem anderen Nummerierungsschema hinzu
            // Da wir nicht hinzufügen können, verwenden wir den nächsten verfügbaren Absatz
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Zeige den Aufzählungstyp (schreibgeschützte Eigenschaft)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Füge Text zum zweiten Absatz hinzu
            shape.TextBody.Text += "\nSecond Item";

            // Speichere die Arbeitsmappe, um die Aufzählungseffekte zu demonstrieren
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Siehe auch

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


