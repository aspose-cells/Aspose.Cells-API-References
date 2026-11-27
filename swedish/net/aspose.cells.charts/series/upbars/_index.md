---
title: "Series.UpBars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Returnerar ett DropBars-objekt som representerar uppåtriktade staplar i ett linjediagram. Gäller endast för linjediagram"
type: docs
url: /sv/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Returnerar ett DropBars‑objekt som representerar uppåtriktade staplar i ett linjediagram. Gäller endast linjediagram.

```csharp
public DropBars UpBars { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyUpBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldatat för linjediagram med upp/ner-staplar
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Aktivera och anpassa uppstaplar
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### Se även

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


