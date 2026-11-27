---
title: "PlotArea.IsAutomaticSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PlotArea‑egenskap. Anger om plotområdet är automatiskt storleksanpassat"
type: docs
url: /sv/net/aspose.cells.charts/plotarea/isautomaticsize/
---
## PlotArea.IsAutomaticSize property

Anger om plotområdet är automatiskt storleksanpassat.

```csharp
public override bool IsAutomaticSize { get; set; }
```

### Anmärkningar

OBS: När IsAutomaticSize sätts till True, kommer de värden du manuellt angivit för Width och Height att inaktiveras.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera plot-området
            PlotArea plotArea = chart.PlotArea;
            plotArea.IsAutomaticSize = false; // Disable automatic sizing
            plotArea.Width = 3000;
            plotArea.Height = 2000;

            workbook.Save("PlotAreaIsAutomaticSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


