---
title: "Class Marker"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.Marker class. Rappresenta il marcatore in un grafico a linee, a dispersione o radar"
type: docs
url: /it/net/aspose.cells.charts/marker/
---
## Marker class

Rappresenta il marcatore in un grafico a linee, a dispersione o radar.

```csharp
public class Marker
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Ottiene il [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Rappresenta il colore di sfondo del marcatore in un grafico a linee, a dispersione o radar. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Ottiene o imposta il tipo di impostazione del colore di sfondo del marcatore. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Ottiene il [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Rappresenta il colore di primo piano del marcatore in un grafico a linee, a dispersione o radar. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Ottiene o imposta il tipo di impostazione del colore di primo piano del marcatore. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Rappresenta la dimensione del marcatore in unità di punti. Si applica a grafico a linee, grafico a dispersione o grafico radar. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Rappresenta la dimensione del marcatore in unità di pixel. Si applica a grafici a linee, grafici a dispersione o grafici radar. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Rappresenta lo stile del marcatore. Si applica a un grafico a linee, un grafico a dispersione o un grafico radar. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Ottieni il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accedi alla prima serie
            Series series = chart.NSeries[0];

            // Imposta le proprietà del marcatore
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Salva la cartella di lavoro
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


