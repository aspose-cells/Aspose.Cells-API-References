---
title: "Marker.BackgroundColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Marker. Rappresenta il colore di sfondo del marcatore in un grafico a linee, a dispersione o radar"
type: docs
url: /it/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Rappresenta il colore di sfondo del marcatore in un grafico a linee, a dispersione o radar.

```csharp
public Color BackgroundColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Personalizza l'aspetto del marcatore
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


