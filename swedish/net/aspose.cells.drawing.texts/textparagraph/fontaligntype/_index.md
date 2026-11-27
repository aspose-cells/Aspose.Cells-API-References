---
title: "TextParagraph.FontAlignType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Bestämmer var vertikalt på en textrad de faktiska orden placeras. Detta hanterar vertikal placering av tecknen i förhållande till baslinjerna."
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Bestämmer var vertikalt på en textrad de faktiska orden placeras. Detta hanterar vertikal placering av tecknen i förhållande till baslinjerna.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFontAlignTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Hämta det första stycket i textrutan
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Visa det aktuella värdet för FontAlignType
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Ställ in FontAlignType till Nederst
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Ställ in FontAlignType till Centrerad
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Ställ in FontAlignType till Överst
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Spara arbetsboken för att se effekterna
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


