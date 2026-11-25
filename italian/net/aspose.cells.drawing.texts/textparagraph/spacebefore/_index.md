---
title: "TextParagraph.SpaceBefore"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/spacebefore/
---
## TextParagraph.SpaceBefore property

Ottiene e imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo.

```csharp
public double SpaceBefore { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo e imposta il testo
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Recupera i paragrafi
            Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configura la spaziatura del secondo paragrafo
            Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4; // Demonstrate SpaceBefore property
            
            // Salva e verifica
            string outputPath = "output_SpaceBeforeDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Demo completed. File saved: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


