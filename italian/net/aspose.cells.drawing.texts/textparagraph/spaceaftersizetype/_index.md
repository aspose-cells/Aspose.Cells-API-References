---
title: "TextParagraph.SpaceAfterSizeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Ottiene e imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceAfterSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo e imposta il testo con più paragrafi
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Ottieni il secondo paragrafo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Imposta le proprietà di spaziatura con il tipo di dimensione
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfter = 10; // 10 points space after
            
            // Salva e ricarica per verificare
            string filePath = "TextParagraphPropertySpaceAfterSizeTypeDemo_Output.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
        }
    }
}
```

### Vedi anche

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


