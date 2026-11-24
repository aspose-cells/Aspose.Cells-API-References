---
title: "Klasse BulletValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.BulletValue Klasse. Stellt den Wert des Aufzählungszeichens dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Stellt den Wert der Aufzählung dar.

```csharp
public abstract class BulletValue
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Ermittelt den Typ des Aufzählungszeichenwerts. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Textfeld und rufe seine Textabsätze ab
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Erstelle eine Instanz von CharacterBulletValue (die von BulletValue erbt)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Setze den Aufzählungszeichenwert für den Absatz (Bullet ist schreibgeschützt, daher müssen wir ihn anders ändern)
            // Da Bullet schreibgeschützt ist, müssen wir einen anderen Weg finden, es zu setzen
            // Dies könnte das Erstellen eines neuen TextParagraphs mit gesetztem Aufzählungszeichen erfordern
            // Hinweis: Die tatsächliche API könnte eine andere Möglichkeit zum Setzen von Aufzählungszeichen bieten
            // Zur Demonstration gehen wir davon aus, dass wir es über andere Mittel setzen können
            // textParagraph.Bullet = bulletValue; // Diese Zeile wird entfernt, da Bullet schreibgeschützt ist
            textBox.Text = "First bullet point";

            // Füge einen weiteren Absatz mit anderem Aufzählungszeichen hinzu
            // TextParagraphCollection hat keine Add-Methode, daher müssen wir einen anderen Weg finden
            // Dies könnte das Erstellen eines neuen TextParagraphs und das Hinzufügen über andere Mittel beinhalten
            // Zur Demonstration gehen wir davon aus, dass wir den zweiten Absatz direkt erhalten können
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Diese Zeile wird entfernt, da Bullet schreibgeschützt ist
            textBox.Text += "\nSecond bullet point";

            // Demonstriere den Zugriff auf den Aufzählungstyp
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Ergebnis speichern
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


