---
title: "TextTabStopCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TextTabStopCollection. Aggiunge una tabulazione"
type: docs
url: /it/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

Aggiunge un tabulatore.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per aggiungere testo con tabulazioni
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // Ottieni la TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // Chiama il metodo Add con TextTabAlignmentType.Left e posizione 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // Chiama il metodo Add con TextTabAlignmentType.Right e posizione 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // Aggiungi testo con tabulazioni per dimostrare le tabulazioni
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


