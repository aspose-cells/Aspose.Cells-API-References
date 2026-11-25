---
title: "Enum TextNodeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.Texts.TextNodeType. Rappresenta il tipo di nodo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textnodetype/
---
## TextNodeType enumeration

Rappresenta il tipo di nodo.

```csharp
public enum TextNodeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| TextRun | `0` | Rappresenta il nodo di testo. |
| TextParagraph | `1` | Rappresenta il paragrafo di testo. |
| Equation | `2` | Rappresenta il testo dell'equazione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextNodeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una casella di testo e ottieni i suoi paragrafi di testo
            int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.TextBody.AppendText("Sample text with ");
            textbox.TextBody.AppendText("different node types");
            
            // Dimostra l'uso di TextNodeType
            foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
            {
                foreach (FontSetting portion in paragraph.Children)
                {
                    // Ottieni la porzione di testo usando StartIndex e Length
                    string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
                    Console.WriteLine("Text: " + portionText);
                    Console.WriteLine("Node Type: " + portion.Type.ToString());
                    
                    // Esempio di verifica del tipo di nodo
                    if (portion.Type == TextNodeType.TextRun)
                    {
                        portion.Font.Color = System.Drawing.Color.Red;
                    }
                    else if (portion.Type == TextNodeType.Equation)
                    {
                        portion.Font.Color = System.Drawing.Color.Blue;
                    }
                }
            }

            // Salva il risultato
            workbook.Save("TextNodeTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


