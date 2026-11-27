---
title: "TextParagraph.LineSpaceSizeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikalt blankutrymme som ska användas inom ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/linespacesizetype/
---
## TextParagraph.LineSpaceSizeType property

Hämtar och sätter mängden vertikalt blankutrymme som ska användas inom en paragraf.

```csharp
public LineSpaceSizeType LineSpaceSizeType { get; set; }
```

### Exempel

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
            
            // Lägg till en textruta och ange text
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Hämta det andra stycket
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Ange radavståndsegenskaper
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2;
            paragraph.SpaceAfter = 3;
            paragraph.SpaceBefore = 4;
            
            // Spara och exportera
            workbook.Save("TextParagraphPropertyLineSpaceSizeTypeDemo_output.xlsx");
            
            Console.WriteLine("Demo executed successfully. Output file created.");
        }
    }
}
```

### Se även

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


