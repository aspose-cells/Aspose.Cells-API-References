---
title: "Series.DownBars"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Çizgi grafiğindeki aşağı çubukları temsil eden bir DropBars nesnesi döndürür. Yalnızca çizgi grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/downbars/
---
## Series.DownBars property

Çizgi grafiğindeki aşağı çubukları temsil eden bir [`DropBars`](../../dropbars/) nesnesi döndürür. Yalnızca çizgi grafiklerinde uygulanır.

```csharp
public DropBars DownBars { get; }
```

### Örnekler

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

            // Aşağı çubukları etkinleştir ve özelleştir
            chart.NSeries[0].HasUpDownBars = true;
            DropBars downBars = chart.NSeries[0].DownBars;
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            workbook.Save("DownBarsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


