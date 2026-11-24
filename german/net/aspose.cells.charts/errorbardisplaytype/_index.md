---
title: "Enum ErrorBarDisplayType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ErrorBarDisplayType-Enum. Stellt den Anzeigetyp für Fehlermarken dar."
type: docs
url: /de/net/aspose.cells.charts/errorbardisplaytype/
---
## ErrorBarDisplayType enumeration

Stellt den Anzeigetyp der Fehlermarge dar.

```csharp
public enum ErrorBarDisplayType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Both | `0` | Beide |
| Minus | `1` | Minus |
| None | `2` | Keine |
| Plus | `3` | Plus |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDisplayTypeDemo
    {
        public static void ErrorBarDisplayTypeExample()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue(2);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(6);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(7);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Füge ein Säulendiagramm zum Arbeitsblatt hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Konfiguriere Fehlermarken für jede Serie im Diagramm
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorBarDisplayTypeExample.xlsx");
            workbook.Save("ErrorBarDisplayTypeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


