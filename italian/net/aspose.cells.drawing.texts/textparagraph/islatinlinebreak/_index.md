---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica se una parola latina può essere divisa a metà e spostata alla riga successiva senza aggiungere un trattino"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Specifica se una parola latina può essere divisa a metà e spostata alla riga successiva senza aggiungere un trattino.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro (parametri corretti per includere l'altezza)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Ottieni il paragrafo di testo della casella di testo (aggiunto cast esplicito)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // Visualizza il valore corrente di IsLatinLineBreak
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // Imposta IsLatinLineBreak su false (le parole latine non verranno interrotte alla fine della riga)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // Imposta IsLatinLineBreak su true (le parole latine possono essere interrotte alla fine della riga)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


