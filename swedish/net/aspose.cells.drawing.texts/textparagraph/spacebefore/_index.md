---
title: "TextParagraph.SpaceBefore"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikala blanksteg som kommer att finnas före ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/spacebefore/
---
## TextParagraph.SpaceBefore property

Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas före en paragraf.

```csharp
public double SpaceBefore { get; set; }
```

### Exempel

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
            
            // Lägg till textruta och ange text
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Hämta stycken
            Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Konfigurera avståndet för det andra stycket
            Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4; // Demonstrate SpaceBefore property
            
            // Spara och verifiera
            string outputPath = "output_SpaceBeforeDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Demo completed. File saved: " + outputPath);
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


