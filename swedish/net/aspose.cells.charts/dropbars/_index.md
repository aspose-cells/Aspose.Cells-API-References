---
title: "Klass DropBars"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.DropBars-klass. Representerar upp- och nerstaplar i ett diagram"
type: docs
url: /sv/net/aspose.cells.charts/dropbars/
---
## DropBars class

Representerar upp- och nerstaplarna i ett diagram.

```csharp
public class DropBars
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Hämtar [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Hämtar kantens [`Line`](../../aspose.cells.drawing/line/). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till NSeries (diagramdatakälla) till diagrammet som sträcker sig från cellen "A1" till "B3"
            chart.NSeries.Add("A1:B3", true);

            // Aktivera upp- och nerstaplar
            chart.NSeries[0].HasUpDownBars = true;

            // Åtkomst till DropBars-objektet
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Anpassa utseendet på uppstaplarna
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Anpassa utseendet på nerstaplarna
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Spara arbetsboken
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


