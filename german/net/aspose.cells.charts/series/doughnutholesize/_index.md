---
title: "Series.DoughnutHoleSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Gibt die Größe des Lochs in einer Donut‑Diagrammgruppe zurück oder legt sie fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße zwischen 10 und 90 Prozent angegeben."
type: docs
url: /de/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Liefert oder legt die Größe des Lochs in einer Donut‑Diagrammgruppe fest. Die Lochgröße wird als Prozentsatz der Diagrammgröße ausgedrückt, zwischen 10 % und 90 %.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Füge ein Doughnut-Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze die Donut‑Lochgröße (Prozentsatz des Diagrammradius)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Speichere die Arbeitsmappe
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


