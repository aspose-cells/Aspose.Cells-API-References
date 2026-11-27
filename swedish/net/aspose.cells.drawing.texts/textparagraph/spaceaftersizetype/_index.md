---
title: "TextParagraph.SpaceAfterSizeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikalt utrymme som kommer att finnas efter ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas efter en paragraf.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Exempel

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
            
            // Lägg till en textruta och ange text med flera stycken
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Hämta det andra stycket
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Ange avståndsegenskaper med storlekstyp
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfter = 10; // 10 points space after
            
            // Spara och ladda om för att verifiera
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

### Se även

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


