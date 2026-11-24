---
title: "Series.SplitType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Gibt einen Wert zurück oder setzt ihn, der bestimmt, welche Datenpunkte im zweiten Kuchen- oder Balken eines Kuchendiagramms im Kuchen- oder Balkendiagramm liegen."
type: docs
url: /de/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Gibt einen Wert zurück oder setzt ihn, der bestimmt, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
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
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Split‑Typ für die erste Serie festlegen
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


