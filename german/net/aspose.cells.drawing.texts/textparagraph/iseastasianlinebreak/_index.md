---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt an, ob ein ostasiatisches Wort in der Mitte getrennt und in die nächste Zeile umgebrochen werden kann, ohne dass ein Bindestrich hinzugefügt wird."
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Gibt an, ob ein ostasiatisches Wort ohne Hinzufügen eines Bindestrichs am Ende in zwei Teile getrennt und in die nächste Zeile umbrochen werden kann.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Den Textabsatz aus dem ersten Absatz des Textfelds abrufen
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Zeigen Sie den aktuellen Wert von IsEastAsianLineBreak an.
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Setzen Sie IsEastAsianLineBreak auf false (ostasiatische Wörter können getrennt werden).
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Speichern Sie die Arbeitsmappe mit deaktiviertem ostasiatischem Zeilenumbruch.
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Setzen Sie IsEastAsianLineBreak auf true (ostasiatische Wörter werden nicht getrennt).
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Speichern Sie die Arbeitsmappe mit aktiviertem ostasiatischem Zeilenumbruch.
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


