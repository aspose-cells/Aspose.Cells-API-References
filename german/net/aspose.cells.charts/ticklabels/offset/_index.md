---
title: "TickLabels.Offset"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Gibt den Abstand der Labels von der Kategorie-Achse zurück und legt ihn fest. Dies gilt nur für die Kategorie‑x‑Achse"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/offset/
---
## TickLabels.Offset property

Liest und setzt den Abstand der Beschriftungen von der Kategorienachse. Dies gilt nur für die Kategorienachse (x).

```csharp
public int Offset { get; set; }
```

### Hinweise

Der Standardabstand beträgt 100 Prozent, was den Standardabstand zwischen den Achsenbeschriftungen und der Achsenlinie darstellt. Der Wert kann ein ganzzahliger Prozentsatz von 0 bis 1000 sein, relativ zur Schriftgröße der Achsenbeschriftung.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyOffsetDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Zugriff auf die Werteachse
            Axis valueAxis = chart.ValueAxis;
            
            // TickLabels-Offset festlegen
            valueAxis.TickLabels.Offset = 50; // 50% offset from default position

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsOffsetDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


