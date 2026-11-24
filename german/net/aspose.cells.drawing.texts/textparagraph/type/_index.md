---
title: "TextParagraph.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Gibt den Typ des Textknotens zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/type/
---
## TextParagraph.Type property

Ermittelt den Typ des Textknotens.

```csharp
public override TextNodeType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt mit allen erforderlichen Parametern hinzu
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            var textBody = textBox.TextBody;
            textBody.Text = "Sample Text\nSecond Line";

            // Den ersten Absatz aus dem Textkörper abrufen
            var paragraphs = textBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[0];

            // Aktuellen Type-Wert anzeigen
            Console.WriteLine("Current TextNodeType: " + paragraph.Type);

            // Demonstriere, wie die Type-Eigenschaft das Verhalten beeinflusst
            if (paragraph.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("This is a text paragraph node");
                Console.WriteLine("You can access paragraph-specific properties like:");
                Console.WriteLine("AlignmentType: " + paragraph.AlignmentType);
                Console.WriteLine("LineSpace: " + paragraph.LineSpace);
            }
            else if (paragraph.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("This is a simple text run node");
            }
            else if (paragraph.Type == TextNodeType.Equation)
            {
                Console.WriteLine("This is an equation node");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


