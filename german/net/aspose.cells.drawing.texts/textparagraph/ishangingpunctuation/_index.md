---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Gibt an, ob Satzzeichen zwingend in einer Textzeile platziert oder in eine andere Zeile verschoben werden sollen.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Textfeld zum Arbeitsblatt hinzufügen (korrigiert durch Hinzufügen des Höhenparameters)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Den Textabsatz aus dem Textfeld abrufen (korrigiert durch Cast zu TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Den aktuellen Wert von IsHangingPunctuation anzeigen
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // IsHangingPunctuation auf true setzen
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // IsHangingPunctuation auf false setzen
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Die Arbeitsmappe speichern, um die Effekte zu sehen (visuelle Überprüfung erforderlich)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


