---
title: "Klasse TextParagraphCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextParagraphCollection class. Stellt alle Textabsätze dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Stellt alle Textabsätze dar.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Gibt die Anzahl der Textabsätze zurück. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Gibt das [`TextParagraph`](../textparagraph/)‑Objekt an einem bestimmten Index zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Liest den Enumerator der Absätze. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge ein Textfeld zum ersten Arbeitsblatt hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Mehrzeiligen Text festlegen
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Hole die Absatzsammlung
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Greife auf den zweiten Absatz zu und ändere ihn
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


