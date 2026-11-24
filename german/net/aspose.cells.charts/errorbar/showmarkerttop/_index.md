---
title: "ErrorBar.ShowMarkerTTop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ErrorBar-Eigenschaft. Gibt an, ob Fehlerbalken mit einem T-Top formatiert werden."
type: docs
url: /de/net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Gibt an, ob Fehlermargen mit einem T-Oben formatiert werden.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyShowMarkerTTopDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Fügen Sie Beispieldaten hinzu
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(2);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(1);

            // Ein Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdaten festlegen
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Fehlerbalken für die erste Serie konfigurieren
            Series series = chart.NSeries[0];
            series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
            series.YErrorBar.Type = ErrorBarType.Percent;
            series.YErrorBar.Amount = 10;
            
            // Demonstriere die ShowMarkerTTop-Eigenschaft
            series.YErrorBar.ShowMarkerTTop = true;
            series.YErrorBar.Color = System.Drawing.Color.Red;
            series.YErrorBar.Style = LineType.DashDot;

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


