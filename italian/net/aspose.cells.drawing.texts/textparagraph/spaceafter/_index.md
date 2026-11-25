---
title: "TextParagraph.SpaceAfter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

```csharp
public double SpaceAfter { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo e imposta il testo
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Recupera i paragrafi
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Configura la spaziatura del secondo paragrafo
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Salva e verifica
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Ricarica per verificare le impostazioni
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


