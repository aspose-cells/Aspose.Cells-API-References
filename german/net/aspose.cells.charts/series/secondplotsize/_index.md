---
title: "Series.SecondPlotSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Gibt die Größe des sekundären Abschnitts eines Kreis‑in‑Kreis‑Diagramms oder eines Balken‑in‑Kreis‑Diagramms als Prozentsatz der Größe des primären Kreises zurück oder legt sie fest. Kann ein Wert von 5 bis 200 sein."
type: docs
url: /de/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Gibt die Größe des sekundären Abschnitts eines Kreis‑in‑Kreis‑Diagramms oder eines Balken‑in‑Kreis‑Diagramms als Prozentsatz der Größe des primären Kreises zurück oder setzt sie. Kann ein Wert von 5 bis 200 sein.

```csharp
public short SecondPlotSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten für das Kreisdiagramm hinzu.
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie
            Series series = chart.NSeries[0];

            // Setze die SecondPlotSize‑Eigenschaft (Prozentsatz des Kreises, der im zweiten Plot angezeigt wird)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


