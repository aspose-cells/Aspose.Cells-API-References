---
title: "ChartDataTable.BackgroundMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable‑egenskap. Hämtar och anger visningsläget för bakgrunden"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Hämtar och anger visningsläget för bakgrunden

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera datatabell
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Demonstrera användning av BackgroundMode
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.Font.Color = Color.Blue;
            chartTable.HasBorderOutline = true;

            workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


