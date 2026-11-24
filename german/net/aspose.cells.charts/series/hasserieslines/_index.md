---
title: "Series.HasSeriesLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Wahr, wenn ein gestapeltes Säulendiagramm oder Balkendiagramm Serienlinien hat oder wenn ein Pie‑of‑Pie‑Diagramm oder Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulen‑ und Balkendiagramme sowie Pie‑of‑Pie‑ und Bar‑of‑Pie‑Diagramme"
type: docs
url: /de/net/aspose.cells.charts/series/hasserieslines/
---
## Series.HasSeriesLines property

True, wenn ein gestapeltes Säulen‑ oder Balkendiagramm Serienlinien hat oder ein Pie‑of‑Pie‑ bzw. Bar‑of‑Pie‑Diagramm Verbindungslinien zwischen den beiden Abschnitten hat. Gilt nur für gestapelte Säulendiagramme, Balkendiagramme, Pie‑of‑Pie‑Diagramme oder Bar‑of‑Pie‑Diagramme.

```csharp
public bool HasSeriesLines { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasSeriesLinesDemo
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
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Gestapeltes Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.ColumnStacked, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seriendaten hinzufügen
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Zugriff auf die erste Serie
            Series series = chart.NSeries[0];
            
            // Demonstriere die HasSeriesLines‑Eigenschaft
            series.HasSeriesLines = true; // Enable series lines
            
            // Speichere die Arbeitsmappe
            workbook.Save("SeriesHasSeriesLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


