---
title: "Enum TextTabAlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextTabAlignmentType-Enum. Stellt die Text-Tab-Ausrichtungstypen dar."
type: docs
url: /de/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Stellt die Text-Tab-Ausrichtungstypen dar.

```csharp
public enum TextTabAlignmentType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Center | `0` | Der Text an dieser Tabstop-Position ist zentriert ausgerichtet. |
| Decimal | `1` | An dieser Tabstop-Position werden die Dezimalstellen ausgerichtet. |
| Left | `2` | Der Text an dieser Tabstop-Position ist linksbündig ausgerichtet. |
| Right | `3` | Der Text an dieser Tabstop-Position ist rechtsbündig ausgerichtet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie ein Textfeld, um Tab‑Ausrichtungen zu demonstrieren
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Fügen Sie Tabstopps mit verschiedenen Ausrichtungstypen hinzu
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Setzen Sie den Text, um alle Ausrichtungstypen zu demonstrieren
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Wenden Sie Formatierungen an, um die Tabs sichtbar zu machen
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Ergebnis speichern
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


