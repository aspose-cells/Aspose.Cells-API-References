---
title: "TextParagraph.LineSpace"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Hämtar och anger mängden vertikalt blankutrymme som ska användas inom ett stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Hämtar och sätter mängden vertikalt blankutrymme som ska användas inom en paragraf.

```csharp
public double LineSpace { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en textruta
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Kom åt textstyckena
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Konfigurera radavstånd för det andra stycket
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // Spara och ladda om för att demonstrera beständighet
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // Läs om för att verifiera inställningarna
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


