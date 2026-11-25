---
title: "Enum LabelPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.LabelPositionType enum. Rappresenta il tipo di posizione dell'etichetta dati"
type: docs
url: /it/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Rappresenta il tipo di posizione dell'etichetta dei dati.

```csharp
public enum LabelPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Center | `0` | Si applica solo a grafici a barre, a torta 2D/3D |
| InsideBase | `1` | Si applica solo a grafici a barre, a torta 2D/3D |
| InsideEnd | `2` | Si applica solo a grafici a barre |
| OutsideEnd | `3` | Si applica solo a grafici a barre, a torta 2D/3D |
| Above | `4` | Si applica solo a grafici a linee |
| Below | `5` | Si applica solo a grafici a linee |
| Left | `6` | Si applica solo a grafici a linee |
| Right | `7` | Si applica solo a grafici a linee |
| BestFit | `8` | Si applica solo a grafici a torta 2D/3D |
| Moved | `9` | L'utente ha spostato le etichette dei dati. Questo è solo per la lettura del grafico dal file modello. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio per il grafico
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

            // Aggiungi la serie di dati al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dati della prima serie
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Imposta la posizione delle etichette dei dati
            dataLabels.Position = LabelPositionType.InsideBase;

            // Mostra il nome della categoria nelle etichette dei dati
            dataLabels.ShowCategoryName = true;

            // Mostra il valore nelle etichette dei dati
            dataLabels.ShowValue = true;

            // Salva la cartella di lavoro
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


