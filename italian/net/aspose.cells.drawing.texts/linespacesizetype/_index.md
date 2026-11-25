---
title: "Enum LineSpaceSizeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Texts.LineSpaceSizeType enum. Rappresenta il tipo di unità della dimensione dell'interlinea"
type: docs
url: /it/net/aspose.cells.drawing.texts/linespacesizetype/
---
## LineSpaceSizeType enumeration

Rappresenta il tipo di unità della dimensione dell'interlinea.

```csharp
public enum LineSpaceSizeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Percentage | `0` | Rappresenta in unità di una percentuale della dimensione del testo. |
| Points | `1` | Rappresenta in unità di punti. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassLineSpaceSizeTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma di casella di testo
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // Imposta il contenuto del testo
            textBox.Text = "Sample Text\nSecond Line";
            
            // Accedi al primo paragrafo della casella di testo
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];
            
            // Imposta il tipo di dimensione dello spazio dopo a Punti
            paragraph.SpaceAfterSizeType = LineSpaceSizeType.Points;
            
            // Imposta il valore dello spazio dopo (12 punti)
            paragraph.SpaceAfter = 12;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Text box with line spacing created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


