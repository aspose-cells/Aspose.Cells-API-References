---
title: "Enum TextFontAlignType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Texts.TextFontAlignType-Enum. Stellt die verschiedenen Arten der Schriftartausrichtung dar"
type: docs
url: /de/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

Stellt die verschiedenen Arten der Schriftartausrichtung dar.

```csharp
public enum TextFontAlignType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Automatic | `0` | Wenn der Textfluss horizontal oder einfach vertikal ist, entspricht er fontBaseline, bei anderen vertikalen Modi entspricht er fontCenter. |
| Bottom | `1` | Die Buchstaben sind am unteren Ende einer einzelnen Zeile verankert. |
| Baseline | `2` | Die Buchstaben sind an der unteren Grundlinie einer einzelnen Zeile verankert. |
| Center | `3` | Die Buchstaben sind zwischen den beiden Grundlinien einer einzelnen Zeile verankert. |
| Top | `4` | Die Buchstaben sind an der oberen Grundlinie einer einzelnen Zeile verankert. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Textfelder mit unterschiedlichen Schriftartausrichtungen.
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

            // Alle Enum-Werte in der Konsole anzeigen.
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // Speichere die Arbeitsmappe
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


