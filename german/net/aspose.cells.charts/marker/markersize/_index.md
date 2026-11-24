---
title: "Marker.MarkerSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Marker-Eigenschaft. Gibt die Markierungsgröße in Punkt als Einheit an. Gilt für Liniendiagramme, Streudiagramme oder Radar‑Diagramme"
type: docs
url: /de/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Stellt die Markergöße in Punkt als Einheit dar. Gilt für Liniendiagramme, Streudiagramme oder Radar-Diagramme.

```csharp
public int MarkerSize { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Serie hinzufügen – korrigierter Methodenaufruf
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Marker-Eigenschaften festlegen
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


