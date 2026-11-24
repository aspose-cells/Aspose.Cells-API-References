---
title: "TextParagraph.DefaultTabSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt die Standardgröße für ein Tabulatorzeichen in diesem Absatz zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Liest und setzt die Standardgröße für ein Tabulatorzeichen in diesem Absatz.

```csharp
public double DefaultTabSize { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Den Textabsatz aus dem ersten Absatz des Textfelds abrufen
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Den aktuellen Standard-Tabulatorwert anzeigen
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Stellen Sie eine kleinere Tabulatorgröße ein (Standard ist normalerweise etwa 36 Punkte)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Fügen Sie ein weiteres Textfeld mit der Standard-Tabulatorgröße zum Vergleich hinzu
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Speichern Sie die Arbeitsmappe, um den Unterschied im Tab-Abstand zu sehen
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


