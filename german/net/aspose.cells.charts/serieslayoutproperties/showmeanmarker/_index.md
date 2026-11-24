---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SeriesLayoutProperties‑Eigenschaft. Gibt an, ob Marker, die den Mittelwert darstellen, angezeigt werden"
type: docs
url: /de/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Gibt an, ob Marker, die den Mittelwert kennzeichnen, angezeigt werden.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Diagramm erstellen (unter Verwendung des Spalten‑Diagrammtyps, der Mittelwert‑Marker unterstützt)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // Layout‑Eigenschaften mit ShowMeanMarker konfigurieren
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Ausgabe speichern
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### Siehe auch

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


