---
title: "Series.DownBars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Returnerar ett DropBars-objekt som representerar nedåtbalkarna i ett linjediagram. Gäller endast linjediagram"
type: docs
url: /sv/net/aspose.cells.charts/series/downbars/
---
## Series.DownBars property

Returnerar ett [`DropBars`](../../dropbars/) objekt som representerar nedåtbalkarna i ett linjediagram. Gäller endast linjediagram.

```csharp
public DropBars DownBars { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDownBarsDemo
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

            // Aktivera och anpassa nedåtbalkar
            chart.NSeries[0].HasUpDownBars = true;
            DropBars downBars = chart.NSeries[0].DownBars;
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            workbook.Save("DownBarsExample.xlsx");
        }
    }
}
```

### Se även

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


