---
title: "Trendline.DisplayEquation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Trendline-Eigenschaft. Gibt an, ob die Gleichung der Trendlinie im Diagramm im selben Datenbeschriftung wie der Rsquared‑Wert angezeigt wird. Das Setzen dieser Eigenschaft auf True schaltet automatisch Datenbeschriftungen ein"
type: docs
url: /de/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Gibt an, ob die Gleichung für die Trendlinie im Diagramm angezeigt wird (im selben Datenbeschriftung wie der R-Quadrat-Wert). Das Setzen dieser Eigenschaft auf True aktiviert automatisch Datenbeschriftungen.

```csharp
public bool DisplayEquation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Serie und Trendlinie hinzufügen
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Trendlinien‑Eigenschaften konfigurieren
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


