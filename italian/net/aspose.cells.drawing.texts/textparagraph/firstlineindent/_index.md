---
title: "TextParagraph.FirstLineIndent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo nel paragrafo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/firstlineindent/
---
## TextParagraph.FirstLineIndent property

Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo.

```csharp
public double FirstLineIndent { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyFirstLineIndentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 100, 300, 200, 100);
            textBox.Text = "This is a sample paragraph with multiple lines.\nFirst line should have indent.\nSecond line should be normal.";

            // Recupera il paragrafo di testo dalla casella di testo
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visualizza il valore corrente di FirstLineIndent
            Console.WriteLine("Current FirstLineIndent value: " + textParagraph.FirstLineIndent);

            // Imposta un nuovo valore di FirstLineIndent (20 punti)
            textParagraph.FirstLineIndent = 20;
            Console.WriteLine("FirstLineIndent set to: " + textParagraph.FirstLineIndent);

            // Aggiungi un'altra casella di testo per confrontare con l'indentazione predefinita
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 5, 150, 300, 200, 100);
            textBox2.Text = "This is a comparison paragraph without indent.\nFirst line has no indent.\nSecond line is normal.";

            // Salva la cartella di lavoro per vedere gli effetti
            workbook.Save("TextParagraphPropertyFirstLineIndentDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


