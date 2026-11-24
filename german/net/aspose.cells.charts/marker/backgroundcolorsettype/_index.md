---
title: "Marker.BackgroundColorSetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Marker-Eigenschaft. Gibt den Typ der Hintergrundfarbgruppe des Markers zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/marker/backgroundcolorsettype/
---
## Marker.BackgroundColorSetType property

Liest oder setzt den Typ der Hintergrundfarbeneinstellung des Markers.

```csharp
public FormattingType BackgroundColorSetType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorSetTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[seriesIndex];

            // Marker‑Eigenschaften konfigurieren
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;
            series.Marker.BackgroundColor = System.Drawing.Color.Yellow;

            // Speichere die Arbeitsmappe
            workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


