---
title: "Trendline.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt den Namen der Trendlinie zurück."
type: docs
url: /de/net/aspose.cells.charts/trendline/name/
---
## Trendline.Name property

Gibt den Namen der Trendlinie zurück.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Trendlinie hinzufügen und ihren Namen festlegen.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "My Custom Trendline";
            
            // Speichere die Arbeitsmappe
            workbook.Save("TrendlinePropertyNameDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


