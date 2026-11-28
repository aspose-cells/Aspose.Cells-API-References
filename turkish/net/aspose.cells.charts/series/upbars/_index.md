---
title: "Series.UpBars"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Bir çizgi grafiğindeki yükselen çubukları temsil eden DropBars nesnesini döndürür. Yalnızca çizgi grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Çizgi grafiğindeki yükselen çubukları temsil eden bir DropBars nesnesi döndürür. Yalnızca çizgi grafiklerine uygulanır.

```csharp
public DropBars UpBars { get; }
```

### Örnekler

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

            // Yukarı/aşağı çubuklu çizgi grafik için örnek veri
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Yukarı çubukları etkinleştir ve özelleştir
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


