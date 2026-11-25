---
title: "TextParagraph.LineSpaceSizeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/linespacesizetype/
---
## TextParagraph.LineSpaceSizeType property

Ottiene e imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo e imposta il testo
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Ottieni il secondo paragrafo
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Imposta le proprietà dell'interlinea
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2;
            paragraph.SpaceAfter = 3;
            paragraph.SpaceBefore = 4;
            
            // Salva ed esporta
            workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
            
            Console.WriteLine("Demo executed successfully. Output file created.");
        }
    }
}
```

### Vedi anche

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


