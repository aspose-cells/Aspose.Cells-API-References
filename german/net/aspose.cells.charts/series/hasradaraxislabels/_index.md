---
title: "Series.HasRadarAxisLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Wahr, wenn ein Radar-Diagramm Kategorienachsenbeschriftungen hat. Gilt nur für Radar-Diagramme"
type: docs
url: /de/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

True, wenn ein Radar‑Diagramm Kategorienachsen‑Beschriftungen hat. Gilt nur für Radar‑Diagramme.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasRadarAxisLabelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten für das Radar-Diagramm hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // Ein Radar‑Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seriendaten hinzufügen
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Holen Sie die Serie und setzen Sie Radar-Achsenbeschriftungen
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // Speichere die Arbeitsmappe
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


