---
title: "ChartDataTable.BackgroundMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Arka planın görüntüleme modunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Arka planın görüntüleme modunu alır ve ayarlar

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Örnekler

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

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Veri tablosunu yapılandır
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // BackgroundMode kullanımını göster
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.Font.Color = Color.Blue;
            chartTable.HasBorderOutline = true;

            workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


