---
title: "Enum ChartMarkerType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.ChartMarkerType. Rappresenta lo stile del marcatore in un grafico a linee, grafico a dispersione o grafico radar."
type: docs
url: /it/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Rappresenta lo stile del marcatore in un grafico a linee, a dispersione o radar.

```csharp
public enum ChartMarkerType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Marcatori automatici. |
| Circle | `1` | Marcatori circolari. |
| Dash | `2` | Marcatori a barra lunga |
| Diamond | `3` | Marcatori a forma di diamante. |
| Dot | `4` | Marcatori a barra corta. |
| None | `5` | Nessun marcatore. |
| SquarePlus | `6` | Marcatori quadrati con segno più. |
| Square | `7` | Marcatori quadrati. |
| SquareStar | `8` | Marcatori quadrati con asterisco. |
| Triangle | `9` | Indicatori triangolari. |
| SquareX | `10` | Indicatori quadrati con una X. |
| Picture | `11` | Immagine |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi la serie di dati al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi all'indicatore della prima serie
            Marker marker = chart.NSeries[0].Marker;

            // Imposta lo stile dell'indicatore
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Imposta la dimensione dell'indicatore
            marker.MarkerSize = 10;

            // Imposta i colori di primo piano e di sfondo dell'indicatore
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


