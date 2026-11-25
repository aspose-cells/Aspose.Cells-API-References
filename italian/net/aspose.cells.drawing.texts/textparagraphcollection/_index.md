---
title: "Classe TextParagraphCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.TextParagraphCollection classe. Rappresenta tutti i paragrafi di testo."
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Rappresenta tutti i paragrafi di testo.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Ottiene il conteggio dei paragrafi di testo. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Ottiene l'oggetto [`TextParagraph`](../textparagraph/) a un indice specifico. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Ottiene l'enumeratore dei paragrafi. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una casella di testo al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Imposta testo multilinea
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Ottieni la raccolta di paragrafi
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Accedi e modifica il secondo paragrafo
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Salva la cartella di lavoro
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


