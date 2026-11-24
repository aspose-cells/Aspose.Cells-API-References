---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt an, ob ein lateinisches Wort in der Mitte getrennt und ohne Hinzufügen eines Bindestrichs in die nächste Zeile umgebrochen werden kann"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Gibt an, ob ein lateinisches Wort ohne Hinzufügen eines Bindestrichs am Ende in zwei Teile getrennt und in die nächste Zeile umbrochen werden kann.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein Textfeld zum Arbeitsblatt hinzufügen (Parameter korrigiert, um Höhe einzuschließen)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Den Textabsatz des Textfelds abrufen (expliziter Cast hinzugefügt)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // Den aktuellen Wert von IsLatinLineBreak anzeigen
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // IsLatinLineBreak auf false setzen (Lateinische Wörter werden am Zeilenende nicht umbrochen)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // IsLatinLineBreak auf true setzen (Lateinische Wörter können am Zeilenende umbrochen werden)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


