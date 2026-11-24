---
title: "TextParagraph.FontAlignType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraph-Eigenschaft. Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert sind. Dies befasst sich mit der vertikalen Platzierung der Zeichen in Bezug auf die Grundlinien."
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Bestimmt, wo vertikal in einer Textzeile die eigentlichen Wörter positioniert sind. Dies betrifft die vertikale Anordnung der Zeichen in Bezug auf die Grundlinien.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Textfeld zum Arbeitsblatt hinzu
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Holen Sie den ersten Absatz des Textfelds.
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Zeigen Sie den aktuellen FontAlignType-Wert an.
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Setzen Sie FontAlignType auf Bottom.
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Setzen Sie FontAlignType auf Center.
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Setzen Sie FontAlignType auf Top.
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Speichere die Arbeitsmappe, um die Auswirkungen zu sehen
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


