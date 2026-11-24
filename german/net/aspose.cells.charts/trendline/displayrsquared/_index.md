---
title: "Trendline.DisplayRSquared"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt an, ob der Rsquared-Wert der Trendlinie im Diagramm im selben Datenbeschriftung wie die Gleichung angezeigt wird. Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein."
type: docs
url: /de/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Gibt an, ob der R-Quadrat-Wert der Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie die Gleichung). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

```csharp
public bool DisplayRSquared { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Eine Trendlinie hinzufügen und sie über den Index abrufen.
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // DisplayRSquared-Eigenschaft demonstrieren.
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Speichere die Arbeitsmappe
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


