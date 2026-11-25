---
title: "TextParagraph.AlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta il tipo di allineamento orizzontale del testo del paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Ottiene e imposta il tipo di allineamento orizzontale del testo del paragrafo.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma di casella di testo
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "First Line\nSecond Line\nThird Line";
            
            // Ottieni i paragrafi di testo
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
            
            // Imposta un allineamento diverso per ogni paragrafo
            paragraphs[0].AlignmentType = TextAlignmentType.Center;
            paragraphs[1].AlignmentType = TextAlignmentType.Left;
            paragraphs[2].AlignmentType = TextAlignmentType.Right;
            
            // Salva la cartella di lavoro
            workbook.Save("TextParagraphAlignmentDemo.xlsx");
            
            Console.WriteLine("Text paragraph alignment demo completed successfully.");
        }
    }
}
```

### Vedi anche

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


