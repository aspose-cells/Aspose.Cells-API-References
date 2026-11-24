---
title: "TextParagraph.AlignmentType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt den horizontalen Ausrichtungstyp des Textes im Absatz zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Liest und setzt den horizontalen Ausrichtungstyp des Textes im Absatz.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine Textfeldform hinzu
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "First Line\nSecond Line\nThird Line";
            
            // Textabsätze abrufen
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
            
            // Unterschiedliche Ausrichtung für jeden Absatz festlegen
            paragraphs[0].AlignmentType = TextAlignmentType.Center;
            paragraphs[1].AlignmentType = TextAlignmentType.Left;
            paragraphs[2].AlignmentType = TextAlignmentType.Right;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphAlignmentDemo.xlsx");
            
            Console.WriteLine("Text paragraph alignment demo completed successfully.");
        }
    }
}
```

### Siehe auch

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


