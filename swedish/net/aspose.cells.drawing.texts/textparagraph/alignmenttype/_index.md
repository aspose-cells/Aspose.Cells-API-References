---
title: "TextParagraph.AlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger den horisontella justeringstypen för texten i stycket"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Hämtar och sätter den horisontella justeringstypen för texten i paragrafen.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "First Line\nSecond Line\nThird Line";
            
            // Hämta textstyckena
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
            
            // Ange olika justeringar för varje stycke
            paragraphs[0].AlignmentType = TextAlignmentType.Center;
            paragraphs[1].AlignmentType = TextAlignmentType.Left;
            paragraphs[2].AlignmentType = TextAlignmentType.Right;
            
            // Spara arbetsboken
            workbook.Save("TextParagraphAlignmentDemo.xlsx");
            
            Console.WriteLine("Text paragraph alignment demo completed successfully.");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


