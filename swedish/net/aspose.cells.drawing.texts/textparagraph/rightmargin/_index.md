---
title: "TextParagraph.RightMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Anger högermarginalen för stycket"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/rightmargin/
---
## TextParagraph.RightMargin property

Anger högermarginalen för paragrafen.

```csharp
public double RightMargin { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyRightMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "This is a sample text to demonstrate RightMargin property of TextParagraph.";

            // Hämta textstycket från textrutans första stycke
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visa det aktuella värdet för högermarginalen
            Console.WriteLine("Current RightMargin value: " + paragraph.RightMargin);

            // Ställ in ett nytt värde för högermarginalen (i punkter)
            paragraph.RightMargin = 20.0;

            // Lägg till en annan textruta för att visa skillnaden
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 2, 1, 2, 200, 200);
            textBox2.Text = "This text has default RightMargin for comparison.";
            
            // Spara arbetsboken för att se effekten
            workbook.Save("TextParagraphRightMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


