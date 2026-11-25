---
title: "TextParagraph.LeftMargin"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica il margine sinistro del paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Specifica il margine sinistro del paragrafo.

```csharp
public double LeftMargin { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Ottieni il paragrafo di testo dal primo paragrafo della casella di testo
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visualizza il valore corrente del margine sinistro
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Imposta un nuovo valore del margine sinistro (in punti)
            paragraph.LeftMargin = 20.0;

            // Dimostra l'effetto aggiungendo un'altra casella di testo con il margine predefinito
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Salva la cartella di lavoro per mostrare la differenza
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


