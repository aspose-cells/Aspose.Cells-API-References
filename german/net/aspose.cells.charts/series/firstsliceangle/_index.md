---
title: "Series.FirstSliceAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt den Winkel des ersten Stücks eines Kreis‑ oder Donutdiagramms in Grad im Uhrzeigersinn von der Vertikalen zurück oder legt ihn fest. Gilt nur für Kreis‑, 3D‑Kreis‑ und Donut‑Diagramme mit Werten von 0 bis 360"
type: docs
url: /de/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Liest oder legt den Winkel des ersten Kuchen‑ oder Donutscheibens in Grad fest (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen-, 3‑D‑Kuchen‑ und Donutdiagramme, mit Werten von 0 bis 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für das Kreisdiagramm hinzu.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Kuchendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie und setze FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


