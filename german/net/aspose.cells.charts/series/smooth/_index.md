---
title: "Series.Smooth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Stellt die Kurvenglättung dar. Wahr, wenn die Kurvenglättung für das Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien."
type: docs
url: /de/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Stellt die Kurvenglättung dar. Wahr, wenn die Kurvenglättung für ein Liniendiagramm oder Streudiagramm aktiviert ist. Gilt nur für Liniendiagramme und Streudiagramme mit Linien.

```csharp
public bool Smooth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setzen Sie die Smooth-Eigenschaft für die erste Serie
            chart.NSeries[0].Smooth = true;

            // Speichere die Arbeitsmappe
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


