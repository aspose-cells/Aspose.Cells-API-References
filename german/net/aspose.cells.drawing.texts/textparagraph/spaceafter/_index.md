---
title: "TextParagraph.SpaceAfter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt die Menge des vertikalen Leerraums an, die nach einem Absatz vorhanden sein wird, und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/spaceafter/
---
## TextParagraph.SpaceAfter property

Liest und setzt die Menge des vertikalen Leerraums, die nach einem Absatz vorhanden sein wird.

```csharp
public double SpaceAfter { get; set; }
```

### Beispiele

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
            
            // Fügen Sie ein Textfeld hinzu und setzen Sie den Text
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Absätze abrufen
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Den Abstand des zweiten Absatzes konfigurieren
            TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3; // Demonstrate SpaceAfter property
            p.SpaceBefore = 4;
            
            // Speichern und überprüfen
            workbook.Save("TextParagraphPropertySpaceAfterDemo.xlsx");
            
            // Neu laden, um die Einstellungen zu überprüfen
            Workbook loadedWorkbook = new Workbook("TextParagraphPropertySpaceAfterDemo.xlsx");
            TextParagraph loadedPara = loadedWorkbook.Worksheets[0].Shapes[0].TextBody.TextParagraphs[1];
            
            Console.WriteLine("SpaceAfter: " + loadedPara.SpaceAfter);
            Console.WriteLine("SpaceBefore: " + loadedPara.SpaceBefore);
            Console.WriteLine("LineSpace: " + loadedPara.LineSpace);
        }
    }
}
```

### Siehe auch

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


