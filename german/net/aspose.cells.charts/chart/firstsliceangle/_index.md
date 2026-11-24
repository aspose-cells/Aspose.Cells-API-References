---
title: "Chart.FirstSliceAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Diagramm-Eigenschaft. Gibt den Winkel des ersten Kuchen- oder Donut-Diagrammsegments in Grad im Uhrzeigersinn von der Vertikalen zurück oder setzt ihn. Gilt nur für Kuchen-, 3D-Kuchen- und Donut-Diagramme von 0 bis 360."
type: docs
url: /de/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Liefert oder setzt den Winkel des ersten Kuchen‑ oder Donut‑Diagrammsegments in Grad (im Uhrzeigersinn von vertikal). Gilt nur für Kuchen-, 3‑D‑Kuchen‑ und Donut‑Diagramme, 0 bis 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Kuchendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Datenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ersten Segmentwinkel auf 45 Grad setzen
            chart.FirstSliceAngle = 45;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Siehe auch

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


