---
title: "Enum TickLabelAlignmentType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.TickLabelAlignmentType enum. Rappresenta il tipo di allineamento del testo per le etichette dei tick sull'asse"
type: docs
url: /it/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Rappresenta il tipo di allineamento del testo per le etichette dei segni sull'asse

```csharp
public enum TickLabelAlignmentType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Center | `0` | Specifica che il testo è centrato. |
| Left | `1` | Specifica che il testo è allineato a sinistra. |
| Right | `2` | Specifica che il testo è allineato a destra.. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
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

            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dei tick dell'asse delle categorie
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Imposta il tipo di allineamento per le etichette dei tick
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Salva la cartella di lavoro
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


