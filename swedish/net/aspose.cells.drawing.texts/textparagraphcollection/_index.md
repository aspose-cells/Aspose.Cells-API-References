---
title: "Class TextParagraphCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextParagraphCollection class. Representerar alla textstycken"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

Representerar alla textstycken.

```csharp
public class TextParagraphCollection : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | Hämtar antalet textstycken. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | Hämtar [`TextParagraph`](../textparagraph/) objektet på ett specifikt index. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | Hämtar enumeratorn för styckena. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en textruta i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // Ställ in flerradig text
            shape.Text = "First paragraph\nSecond paragraph";
            
            // Hämta styckeskollektionen
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // Kom åt och ändra det andra stycket
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // Spara arbetsboken
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


