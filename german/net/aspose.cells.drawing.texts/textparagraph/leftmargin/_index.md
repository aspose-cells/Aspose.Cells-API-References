---
title: "TextParagraph.LeftMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt den linken Rand des Absatzes an"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Gibt den linken Rand des Absatzes an.

```csharp
public double LeftMargin { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Den Textabsatz aus dem ersten Absatz des Textfelds abrufen
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Zeigt den aktuellen Wert des linken Randes an
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Setzt einen neuen Wert für den linken Rand (in Punkten)
            paragraph.LeftMargin = 20.0;

            // Demonstrieren Sie die Wirkung, indem Sie ein weiteres Textfeld mit dem Standardrand hinzufügen
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Speichern Sie die Arbeitsmappe, um den Unterschied zu zeigen
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


