---
title: "Series.DownBars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce un oggetto DropBars che rappresenta le barre discendenti in un grafico a linee. Si applica solo ai grafici a linee"
type: docs
url: /it/net/aspose.cells.charts/series/downbars/
---
## Series.DownBars property

Restituisce un oggetto [`DropBars`](../../dropbars/) che rappresenta le barre discendenti in un grafico a linee. Si applica solo ai grafici a linee.

```csharp
public DropBars DownBars { get; }
```

### Esempi

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

            // Dati di esempio per un grafico a linee con barre su/giù
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Abilita e personalizza le barre discendenti
            chart.NSeries[0].HasUpDownBars = true;
            DropBars downBars = chart.NSeries[0].DownBars;
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            workbook.Save("DownBarsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


