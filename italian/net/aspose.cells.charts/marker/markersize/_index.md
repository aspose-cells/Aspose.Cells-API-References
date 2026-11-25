---
title: "Marker.MarkerSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Marker. Rappresenta la dimensione del marcatore in unità di punti. Si applica a grafici a linee, a dispersione o radar"
type: docs
url: /it/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Rappresenta la dimensione del marcatore in unità di punti. Si applica a grafico a linee, grafico a dispersione o grafico radar.

```csharp
public int MarkerSize { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie - chiamata al metodo corretta
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Imposta le proprietà del marcatore
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Salva la cartella di lavoro
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


