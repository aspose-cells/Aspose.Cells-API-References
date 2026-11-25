---
title: "Enum TextOverflowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.TextOverflowType. Rappresenta il modo in cui il testo trabocca verticalmente o orizzontalmente."
type: docs
url: /it/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Rappresenta il modo in cui il testo trabocca verticalmente o orizzontalmente.

```csharp
public enum TextOverflowType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Clip | `0` | Fai attenzione alle barriere superiori e inferiori. Non fornire alcuna indicazione che esista del testo non visibile. |
| Ellipsis | `1` | Fai attenzione alle barriere superiori e inferiori. Usa un'ellissi per indicare che esiste del testo non visibile. Solo per il trabocco verticale. |
| Overflow | `2` | Fai traboccare il testo e non prestare attenzione alle barriere superiori e inferiori. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi una casella di testo al grafico
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Imposta le proprietà della casella di testo
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Imposta il tipo di trabocco del testo
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Salva la cartella di lavoro
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


