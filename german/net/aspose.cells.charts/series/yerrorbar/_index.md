---
title: "Series.YErrorBar"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series-Eigenschaft. Stellt die Y-Richtung-Fehlerbalken der Series dar."
type: docs
url: /de/net/aspose.cells.charts/series/yerrorbar/
---
## Series.YErrorBar property

Stellt den Y‑Richtungs-Fehlerbalken der Serie dar.

```csharp
public ErrorBar YErrorBar { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyYErrorBarDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Setze YErrorBar-Eigenschaften
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.Type = ErrorBarType.Percent;
            errorBar.Amount = 5;
            errorBar.DisplayType = ErrorBarDisplayType.Both;

            // Speichere die Arbeitsmappe
            workbook.Save("YErrorBarDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


