---
title: "TextParagraph.DefaultTabSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Ottiene e imposta la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo.

```csharp
public double DefaultTabSize { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Ottieni il paragrafo di testo dal primo paragrafo della casella di testo
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visualizza la dimensione predefinita della tabulazione corrente
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Imposta una dimensione della tabulazione più piccola (il valore predefinito è solitamente circa 36 punti)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Aggiungi un'altra casella di testo con la dimensione della tabulazione predefinita per il confronto
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Salva la cartella di lavoro per vedere la differenza nella spaziatura delle tabulazioni
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


