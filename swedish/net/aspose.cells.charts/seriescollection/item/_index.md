---
title: "SeriesCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesCollection‑egenskap. Hämtar Series‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Hämtar [`Series`](../../series/)‑elementet på det angivna indexet.

```csharp
public Series this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Series");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Values");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till den första serien och dess första punkt med Item‑egenskapen
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            // Anpassa punktens utseende
            point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
            point.Area.FillFormat.FillType = FillType.Solid;

            // Spara arbetsboken
            workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


