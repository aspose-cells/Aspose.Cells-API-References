---
title: "TextParagraph.FirstLineIndent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Anger indragstorleken som kommer att tillämpas på den första raden i stycket"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Anger indenteringsstorleken som ska tillämpas på den första textraden i paragrafen.

```csharp
public double FirstLineIndent { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Hämta textstycket från textrutan
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visa aktuellt FirstLineIndent‑värde
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Ställ in ett nytt FirstLineIndent‑värde (20 punkter)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Lägg till en annan textruta för att jämföra med standardindrag
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Spara arbetsboken för att se effekterna
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


