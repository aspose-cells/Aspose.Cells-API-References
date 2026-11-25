---
title: "Series.HasUpDownBars"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. True se un grafico a linee ha barre su e giù. Si applica solo ai grafici a linee"
type: docs
url: /it/net/aspose.cells.charts/series/hasupdownbars/
---
## Series.HasUpDownBars property

Vero se un grafico a linee ha barre su e giù. Si applica solo ai grafici a linee.

```csharp
public bool HasUpDownBars { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasUpDownBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("A1:B3", true);
            chart.NSeries[0].HasUpDownBars = true;

            Aspose.Cells.Charts.DropBars upBars = chart.NSeries[0].UpBars;
            Aspose.Cells.Charts.DropBars downBars = chart.NSeries[0].DownBars;

            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            workbook.Save("SeriesPropertyHasUpDownBarsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


