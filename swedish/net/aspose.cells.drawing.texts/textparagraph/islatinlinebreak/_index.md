---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextParagraph-egenskap. Anger om ett latinskt ord kan brytas i två delar och flyttas till nästa rad utan att ett bindestreck läggs till"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Anger om ett latinskt ord kan brytas i två delar och radbrytas till nästa rad utan att ett bindestreck läggs till.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en textruta i kalkylbladet (fixade parametrar för att inkludera höjd)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Hämta textstycket i textrutan (tillägg av explicit typkonvertering)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // Visa det aktuella värdet för IsLatinLineBreak
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // Ställ in IsLatinLineBreak till false (latinska ord bryts inte vid radslut)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // Ställ in IsLatinLineBreak till true (latinska ord kan brytas vid radslut)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Se även

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


