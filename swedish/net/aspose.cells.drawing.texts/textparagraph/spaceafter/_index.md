---
title: "TextParagraph.SpaceAfter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikalt utrymme som kommer att finnas efter ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas efter en paragraf.

```csharp
public double SpaceAfter { get; set; }
```

### Exempel

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
            
            // Lägg till textruta och ange text
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Hämta stycken
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Konfigurera avståndet för det andra stycket
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Spara och verifiera
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Läs om för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


