---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph-egenskap. Anger om interpunktion ska tvingas placeras på samma rad som texten eller på en separat rad"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Anger om interpunktion ska tvingas placeras på samma rad som texten eller sättas på en annan rad.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet (fixerat genom att lägga till höjdparameter)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Hämta textstycket från textrutan (fixerat genom att kasta till TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visa det aktuella värdet för IsHangingPunctuation
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // Ställ in IsHangingPunctuation till true
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Ställ in IsHangingPunctuation till false
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Spara arbetsboken för att se effekterna (visuell inspektion krävs)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


