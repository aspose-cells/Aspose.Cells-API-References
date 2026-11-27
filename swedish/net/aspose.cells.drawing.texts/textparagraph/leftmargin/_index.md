---
title: "TextParagraph.LeftMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Anger vänstermarginalen för stycket"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

Anger vänstermarginalen för paragrafen.

```csharp
public double LeftMargin { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // Hämta textstycket från textrutans första stycke
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visa det aktuella värdet för vänstermarginalen
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // Ställ in ett nytt värde för vänstermarginalen (i punkter)
            paragraph.LeftMargin = 20.0;

            // Demonstrera effekten genom att lägga till en annan textruta med standardmarginal
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // Spara arbetsboken för att visa skillnaden
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


