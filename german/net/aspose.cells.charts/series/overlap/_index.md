---
title: "Series.Overlap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen 100 und 100 sein. Gilt nur für 2D-Balken- und 2D-Säulendiagramme"
type: docs
url: /de/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Gibt an, wie Balken und Säulen positioniert werden. Kann ein Wert zwischen -100 und 100 sein. Gilt nur für 2‑D‑Balken‑ und 2‑D‑Säulendiagramme.

```csharp
public short Overlap { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Fügen Sie ein gruppiertes Säulendiagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze die Overlap‑Eigenschaft für die erste Serie
            chart.NSeries[0].Overlap = -40;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


