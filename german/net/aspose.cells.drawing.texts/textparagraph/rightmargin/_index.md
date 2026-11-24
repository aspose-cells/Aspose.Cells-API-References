---
title: "TextParagraph.RightMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt den rechten Rand des Absatzes an"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Gibt den rechten Rand des Absatzes an.

```csharp
public double RightMargin { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Den Textabsatz aus dem ersten Absatz des Textfelds abrufen
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Zeigt den aktuellen Wert des rechten Randes an
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Setzt einen neuen Wert für den rechten Rand (in Punkten)
            paragraph.RightMargin = 20.0;

            // Fügen Sie ein weiteres Textfeld hinzu, um den Unterschied zu zeigen
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


