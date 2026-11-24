---
title: "TextParagraph.LineSpace"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Liest und setzt die Menge des vertikalen Leerraums, der innerhalb eines Absatzes verwendet wird"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

Liest und setzt die Menge des vertikalen Leerraums, die innerhalb eines Absatzes verwendet wird.

```csharp
public double LineSpace { get; set; }
```

### Beispiele

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
            
            // Fügen Sie eine Textfeldform hinzu
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // Greife auf die Textabsätze zu
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Zeilenabstand für den zweiten Absatz konfigurieren
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // Speichern und neu laden, um die Persistenz zu demonstrieren
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // Neu laden, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


