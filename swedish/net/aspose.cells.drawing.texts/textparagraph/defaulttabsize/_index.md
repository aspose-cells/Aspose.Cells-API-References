---
title: "TextParagraph.DefaultTabSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph-egenskap. Hämtar och anger standardstorleken för ett tabulatortecken i detta stycke"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

Hämtar och sätter standardstorleken för ett tabulatortecken i denna paragraf.

```csharp
public double DefaultTabSize { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Hämta textstycket från textrutans första stycke
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visa den aktuella standardtabbstorleken
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // Ställ in en mindre tabbstorlek (standard är vanligtvis omkring 36 punkter)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // Lägg till en annan textruta med standardtabbstorlek för jämförelse
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // Spara arbetsboken för att se skillnaden i tabulatoravstånd
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


