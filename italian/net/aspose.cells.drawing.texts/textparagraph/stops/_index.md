---
title: "TextParagraph.Stops"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene l'elenco dei tabulatori"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

Ottiene l'elenco dei tabulatori.

```csharp
public TextTabStopCollection Stops { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi testo a una cella e ottieni le sue proprietà di paragrafo di testo
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // Ottieni il paragrafo di testo
            var textOptions = shape.TextBody.TextParagraphs[0];

            // Visualizza il conteggio corrente dei tabulatori
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // Aggiungi nuovi tabulatori
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // Visualizza tabulazioni aggiornate
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


