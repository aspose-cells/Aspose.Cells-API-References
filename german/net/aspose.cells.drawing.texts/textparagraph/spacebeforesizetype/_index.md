---
title: "TextParagraph.SpaceBeforeSizeType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt die Menge des vertikalen Leerraums zurück und legt sie fest, die vor einem Absatz vorhanden sein wird."
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/
---
## TextParagraph.SpaceBeforeSizeType property

Liest und setzt die Menge des vertikalen Leerraums, die vor einem Absatz vorhanden sein wird.

```csharp
public LineSpaceSizeType SpaceBeforeSizeType { get; set; }
```

### Beispiele

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
            
            // Fügen Sie ein Textfeld hinzu und erhalten Sie dessen Form.
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Greifen Sie auf den zweiten Absatz zu.
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[1];
            
            // Legen Sie die Absatzabstandseigenschaften fest.
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceBeforeSizeType = LineSpaceSizeType.Points;
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            paragraph.LineSpace = 12;
            paragraph.SpaceBefore = 8;
            paragraph.SpaceAfter = 10;
            
            // Speichern und neu laden, um die Persistenz zu demonstrieren
            string outputPath = "TextParagraphSpacingDemo.xlsx";
            workbook.Save(outputPath);
            
            // Neu laden, um Eigenschaften zu überprüfen
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

### Siehe auch

* enum [LineSpaceSizeType](../../linespacesizetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


