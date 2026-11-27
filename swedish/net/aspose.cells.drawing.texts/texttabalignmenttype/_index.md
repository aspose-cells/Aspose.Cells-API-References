---
title: "Enum TextTabAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextTabAlignmentType enum. Representerar typerna av textflikjustering"
type: docs
url: /sv/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Representerar typerna av texttabbalignering.

```csharp
public enum TextTabAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Center | `0` | Texten vid detta tabbstopp är centrerad. |
| Decimal | `1` | Vid detta tabbstopp är decimalerna uppradade. |
| Left | `2` | Texten vid detta tabbstopp är vänsterjusterad. |
| Right | `3` | Texten vid detta tabbstopp är högerjusterad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextTabAlignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en textruta för att demonstrera tabbaligneringar
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Lägg till tabbstopp med olika justeringstyper
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Ställ in text för att demonstrera alla justeringstyper
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Applicera formatering för att göra tabbarna synliga
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Spara resultatet
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


