---
title: "Enum TextFontAlignType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Texts.TextFontAlignType enum. Representerar de olika typerna av teckensnittjustering"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

Representerar de olika typerna av teckensnittjustering.

```csharp
public enum TextFontAlignType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Automatic | `0` | När textflödet är horisontellt eller enkelt vertikalt är det samma som fontBaseline, men för andra vertikala lägen är det samma som fontCenter. |
| Bottom | `1` | Bokstäverna är förankrade längst ner på en enda rad. |
| Baseline | `2` | Bokstäverna är förankrade vid den nedre baslinjen på en enda rad. |
| Center | `3` | Bokstäverna är förankrade mellan de två baslinjerna på en enda rad. |
| Top | `4` | Bokstäverna är förankrade vid den övre baslinjen på en enda rad. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextFontAlignTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa textrutor med olika teckensnittjusteringar
            var textBoxAuto = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            textBoxAuto.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Automatic;
            textBoxAuto.Text = "Automatic Alignment";

            var textBoxBottom = worksheet.Shapes.AddTextBox(0, 200, 100, 100, 200, 200);
            textBoxBottom.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Bottom;
            textBoxBottom.Text = "Bottom Alignment";

            var textBoxBaseline = worksheet.Shapes.AddTextBox(0, 400, 100, 100, 200, 200);
            textBoxBaseline.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Baseline;
            textBoxBaseline.Text = "Baseline Alignment";

            var textBoxCenter = worksheet.Shapes.AddTextBox(200, 0, 100, 100, 200, 200);
            textBoxCenter.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Center;
            textBoxCenter.Text = "Center Alignment";

            var textBoxTop = worksheet.Shapes.AddTextBox(200, 200, 100, 100, 200, 200);
            textBoxTop.TextBody.TextParagraphs[0].FontAlignType = TextFontAlignType.Top;
            textBoxTop.Text = "Top Alignment";

            // Visa alla enum‑värden i konsolen
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // Spara arbetsboken
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


