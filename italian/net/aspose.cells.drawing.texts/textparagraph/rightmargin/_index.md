---
title: "TextParagraph.RightMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica il margine destro del paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Specifica il margine destro del paragrafo.

```csharp
public double RightMargin { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Ottieni il paragrafo di testo dal primo paragrafo della casella di testo
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visualizza il valore corrente del margine destro
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Imposta un nuovo valore del margine destro (in punti)
            paragraph.RightMargin = 20.0;

            // Aggiungi un'altra casella di testo per mostrare la differenza
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


