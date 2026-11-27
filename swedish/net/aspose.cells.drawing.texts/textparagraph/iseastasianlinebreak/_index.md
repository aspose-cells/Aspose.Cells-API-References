---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph egenskap. Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till."
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Anger om ett östasiatiskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Hämta textstycket från textrutans första stycke
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visa det aktuella värdet för IsEastAsianLineBreak
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Ställ in IsEastAsianLineBreak till false (östasiatiska ord kan brytas)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Spara arbetsboken med östasiatiskt radbrytning inaktiverat
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Ställ in IsEastAsianLineBreak till true (östasiatiska ord kommer inte att brytas)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Spara arbetsboken med östasiatiskt radbrytning aktiverat
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


