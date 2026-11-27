---
title: "TextParagraph.SpaceBeforeSizeType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikala blanksteg som kommer att finnas före ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/
---
## TextParagraph.SpaceBeforeSizeType property

Hämtar och sätter mängden vertikalt blankutrymme som kommer att finnas före en paragraf.

```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeSizeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta och hämta dess form
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Åtkomst till det andra stycket
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Ställ in egenskaper för styckeavstånd
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            paragraph.LineSpace = 12;
            paragraph.SpaceBefore = 8;
            paragraph.SpaceAfter = 10;
            
            // Spara och ladda om för att demonstrera beständighet
            string outputPath = "TextParagraphSpacingDemo.xlsx";
            workbook.Save(outputPath);
            
            // Läs om för att verifiera egenskaper
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceBeforeSizeType: " + loadedParagraph.SpaceBeforeSizeType);
            Console.WriteLine("SpaceBefore: " + loadedParagraph.SpaceBefore);
            Console.WriteLine("SpaceAfterSizeType: " + loadedParagraph.SpaceAfterSizeType);
            Console.WriteLine("SpaceAfter: " + loadedParagraph.SpaceAfter);
            Console.WriteLine("LineSpaceSizeType: " + loadedParagraph.LineSpaceSizeType);
            Console.WriteLine("LineSpace: " + loadedParagraph.LineSpace);
        }
    }
}
```

### Se även

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


