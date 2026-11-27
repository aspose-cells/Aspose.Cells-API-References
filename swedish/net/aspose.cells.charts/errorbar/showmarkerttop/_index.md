---
title: "ErrorBar.ShowMarkerTTop"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ErrorBar-egenskap. Anger om felstaplar formateras med en Ttop"
type: docs
url: /sv/net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Indikerar om felstaplar formateras med en T-top.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(2);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(1);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagramdata
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Konfigurera felstaplar för den första serien
            Series series = chart.NSeries[0];
            series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
            series.YErrorBar.Type = ErrorBarType.Percent;
            series.YErrorBar.Amount = 10;
            
            // Demonstrera ShowMarkerTTop-egenskapen
            series.YErrorBar.ShowMarkerTTop = true;
            series.YErrorBar.Color = System.Drawing.Color.Red;
            series.YErrorBar.Style = LineType.DashDot;

            // Spara arbetsboken
            workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
        }
    }
}
```

### Se även

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


