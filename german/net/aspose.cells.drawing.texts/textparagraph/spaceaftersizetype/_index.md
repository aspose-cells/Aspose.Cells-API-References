---
title: "TextParagraph.SpaceAfterSizeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt die Menge des vertikalen Leerraums an, die nach einem Absatz vorhanden sein wird, und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/
---
## TextParagraph.SpaceAfterSizeType property

Liest und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden sein wird.

```csharp
public LineSpaceSizeType SpaceAfterSizeType { get; set; }
```

### Beispiele

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
            
            // Füge ein Textfeld hinzu und setze Text mit mehreren Absätzen
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Den zweiten Absatz abrufen
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Lege Abstandseigenschaften mit Größentyp fest
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfter = 10; // 10 points space after
            
            // Speichern und neu laden, um zu überprüfen
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

### Siehe auch

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


