---
title: "TextTabStopCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextTabStopCollection. Ottiene TextTabStop per indice"
type: docs
url: /it/net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

Ottiene [`TextTabStop`](../../texttabstop/) per indice.

```csharp
public TextTabStop this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo contenente caratteri di tabulazione
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // Accedi alla raccolta di tabulazioni del primo paragrafo
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // Prepara la raccolta con tabulazioni note
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // Usa la proprietà Item (indicizzatore) per leggere una specifica tabulazione
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // Dimostra la lettura di un altro elemento
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // Salva la cartella di lavoro con le modifiche
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


