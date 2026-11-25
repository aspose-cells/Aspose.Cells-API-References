---
title: "TextParagraph.FontAlignType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Determina dove verticalmente su una riga di testo le parole effettive sono posizionate. Questo riguarda il posizionamento verticale dei caratteri rispetto alle linee di base"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/fontaligntype/
---
## TextParagraph.FontAlignType property

Determina dove, verticalmente, su una riga di testo, le parole effettive sono posizionate. Questo riguarda il posizionamento verticale dei caratteri rispetto alle linee di base.

```csharp
public TextFontAlignType FontAlignType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textboxIndex = worksheet.TextBoxes.Add(1, 1, 200, 400);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample Text\nFor Font Alignment Demo";

            // Ottieni il primo paragrafo della casella di testo
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];

            // Visualizza il valore corrente di FontAlignType
            Console.WriteLine("Current FontAlignType value: " + paragraph.FontAlignType);

            // Imposta FontAlignType su Bottom
            paragraph.FontAlignType = TextFontAlignType.Bottom;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Imposta FontAlignType su Center
            paragraph.FontAlignType = TextFontAlignType.Center;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Imposta FontAlignType su Top
            paragraph.FontAlignType = TextFontAlignType.Top;
            Console.WriteLine("FontAlignType set to: " + paragraph.FontAlignType);

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("TextParagraphPropertyFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextFontAlignType](../../textfontaligntype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


