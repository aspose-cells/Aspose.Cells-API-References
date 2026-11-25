---
title: "Enum TextFontAlignType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextFontAlignType. Rappresenta i diversi tipi di allineamento del carattere"
type: docs
url: /it/net/aspose.cells.drawing.texts/textfontaligntype/
---
## TextFontAlignType enumeration

Rappresenta i diversi tipi di allineamento del carattere.

```csharp
public enum TextFontAlignType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Quando il flusso di testo è orizzontale o verticale semplice è lo stesso di fontBaseline, ma per le altre modalità verticali è lo stesso di fontCenter. |
| Bottom | `1` | Le lettere sono ancorate all'estremità inferiore di una singola riga. |
| Baseline | `2` | Le lettere sono ancorate alla linea di base inferiore di una singola riga. |
| Center | `3` | Le lettere sono ancorate tra le due linee di base di una singola riga. |
| Top | `4` | Le lettere sono ancorate alla linea di base superiore di una singola riga. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea caselle di testo con diversi allineamenti del font
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

            // Visualizza tutti i valori enum nella console
            Console.WriteLine("TextFontAlignType values:");
            Console.WriteLine($"Automatic: {TextFontAlignType.Automatic}");
            Console.WriteLine($"Bottom: {TextFontAlignType.Bottom}");
            Console.WriteLine($"Baseline: {TextFontAlignType.Baseline}");
            Console.WriteLine($"Center: {TextFontAlignType.Center}");
            Console.WriteLine($"Top: {TextFontAlignType.Top}");

            // Salva la cartella di lavoro
            workbook.Save("TextFontAlignTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


