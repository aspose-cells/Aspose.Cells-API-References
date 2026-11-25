---
title: "TextParagraph.LineSpace"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

```csharp
public double LineSpace { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma di casella di testo
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Accedi ai paragrafi di testo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configura l'interlinea per il secondo paragrafo
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // Salva e ricarica per dimostrare la persistenza
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // Ricarica per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


