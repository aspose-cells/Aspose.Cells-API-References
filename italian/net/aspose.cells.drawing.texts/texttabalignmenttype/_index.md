---
title: "Enum TextTabAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextTabAlignmentType. Rappresenta i tipi di allineamento delle tabulazioni di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/texttabalignmenttype/
---
## TextTabAlignmentType enumeration

Rappresenta i tipi di allineamento delle tabulazioni di testo.

```csharp
public enum TextTabAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Center | `0` | Il testo a questa tabulazione è allineato al centro. |
| Decimal | `1` | A questa tabulazione, i decimali sono allineati. |
| Left | `2` | Il testo a questa tabulazione è allineato a sinistra. |
| Right | `3` | Il testo a questa tabulazione è allineato a destra. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una casella di testo per dimostrare gli allineamenti delle tabulazioni
            int textBoxIndex = worksheet.TextBoxes.Add(0, 0, 400, 300);
            var textBox = worksheet.TextBoxes[textBoxIndex];
            var paragraph = textBox.TextBody.TextParagraphs[0];

            // Aggiungi tabulazioni con diversi tipi di allineamento
            paragraph.Stops.Add(TextTabAlignmentType.Left, 100);
            paragraph.Stops.Add(TextTabAlignmentType.Center, 200);
            paragraph.Stops.Add(TextTabAlignmentType.Right, 300);
            paragraph.Stops.Add(TextTabAlignmentType.Decimal, 400);

            // Imposta il testo per dimostrare tutti i tipi di allineamento
            textBox.Text = "Left\tCenter\tRight\tDecimal\n" +
                           "Data\tData\tData\t12.34\n" +
                           "More\tMore\tMore\t56.78";

            // Applica la formattazione per rendere le tabulazioni visibili
            textBox.Font.Size = 12;
            textBox.TextBody.TextParagraphs[0].AlignmentType = TextAlignmentType.Left;

            // Salva il risultato
            workbook.Save("TextTabAlignmentTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


