---
title: "Series.HasDropLines"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Wahr, wenn das Diagramm Drop-Linien hat. Gilt nur für Liniendiagramme oder Flächendiagramme."
type: docs
url: /de/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

True, wenn das Diagramm Drop‑Lines hat. Gilt nur für Liniendiagramme oder Flächendiagramme.

```csharp
public bool HasDropLines { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Liniendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Seriendaten hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie
            Series series = chart.NSeries[0];

            // Demonstriere die HasDropLines-Eigenschaft
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Speichere die Arbeitsmappe
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


