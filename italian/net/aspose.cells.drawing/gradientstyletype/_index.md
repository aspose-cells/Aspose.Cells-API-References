---
title: "Enum GradientStyleType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Rappresenta lo stile di sfumatura"
type: docs
url: /it/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Rappresenta lo stile di sfumatura del gradiente.

```csharp
public enum GradientStyleType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DiagonalDown | `0` | Stile di sfumatura diagonale verso il basso |
| DiagonalUp | `1` | Stile di sfumatura diagonale verso l'alto |
| FromCenter | `2` | Stile di sfumatura dal centro |
| FromCorner | `3` | Stile di sfumatura dall'angolo |
| Horizontal | `4` | Stile di sfumatura orizzontale |
| Vertical | `5` | Stile di sfumatura verticale |
| Unknown | `6` | Stile di sfumatura sconosciuto. Solo per lo stile di sfumatura (che non è per alcun membro di GradientStyleType) nel file modello. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);

            // Accedi all'area del tracciato del grafico
            PlotArea plotArea = chart.PlotArea;

            // Accedi al formato di riempimento dell'area del tracciato
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Imposta un riempimento a gradiente bicolore con lo stile DiagonalDown
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Restituisci lo stile di gradiente utilizzato
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Salva la cartella di lavoro
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


