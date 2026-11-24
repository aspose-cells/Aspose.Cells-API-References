---
title: "Series.SplitValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Gibt einen Wert zurück oder setzt ihn, der verwendet wird, um zu bestimmen, welche Datenpunkte im zweiten Kreis- oder Balkendiagramm eines Kreis‑im‑Kreis‑ oder Balken‑im‑Kreis‑Diagramms liegen"
type: docs
url: /de/net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Gibt einen Wert zurück oder setzt ihn, der zur Bestimmung verwendet wird, welche Datenpunkte im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ bzw. Balken‑in‑Kreis‑Diagramms liegen.

```csharp
public double SplitValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);
            worksheet.Cells["B5"].PutValue(50);

            // Ein Kreisdiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Split‑Typ und Wert festlegen
            chart.NSeries[0].SplitType = ChartSplitType.Custom;
            chart.NSeries[0].SplitValue = 20; // Split points with value <= 20

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


