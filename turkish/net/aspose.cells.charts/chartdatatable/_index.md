---
title: "Sınıf ChartDataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartDataTable sınıfı. Bir grafik veri tablosunu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/
---
## ChartDataTable class

Bir grafik veri tablosunu temsil eder.

```csharp
public class ChartDataTable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/chartdatatable/autoscalefont/) { get; set; } | Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'dur. |
| [BackgroundMode](../../aspose.cells.charts/chartdatatable/backgroundmode/) { get; set; } | Arka planın görüntüleme modunu alır ve ayarlar |
| [Border](../../aspose.cells.charts/chartdatatable/border/) { get; } | Nesnenin kenarını temsil eden bir Border nesnesi döndürür |
| [Font](../../aspose.cells.charts/chartdatatable/font/) { get; } | Belirtilen grafik veri tablosunun yazı tipi ayarını temsil eden bir [`Font`](./font/) nesnesi alır. |
| [HasBorderHorizontal](../../aspose.cells.charts/chartdatatable/hasborderhorizontal/) { get; set; } | (**Obsolete.**) Grafik veri tablosunun yatay hücre kenarları varsa doğru |
| [HasBorderOutline](../../aspose.cells.charts/chartdatatable/hasborderoutline/) { get; set; } | (**Obsolete.**) Grafik veri tablosunun dış kenar çizgileri varsa doğru |
| [HasBorderVertical](../../aspose.cells.charts/chartdatatable/hasbordervertical/) { get; set; } | (**Obsolete.**) Grafik veri tablosunun dikey hücre kenarları varsa doğru |
| [HasHorizontalBorder](../../aspose.cells.charts/chartdatatable/hashorizontalborder/) { get; set; } | Grafik veri tablosunun yatay hücre kenarları varsa doğru |
| [HasOutlineBorder](../../aspose.cells.charts/chartdatatable/hasoutlineborder/) { get; set; } | Grafik veri tablosunun dış kenar çizgileri varsa doğru |
| [HasVerticalBorder](../../aspose.cells.charts/chartdatatable/hasverticalborder/) { get; set; } | Grafik veri tablosunun dikey hücre kenarları varsa doğru |
| [ShowLegendKey](../../aspose.cells.charts/chartdatatable/showlegendkey/) { get; set; } | Veri etiketi açıklama anahtarı görünürse doğru. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDataTableDemo
    {
        public static void ChartDataTableExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);

            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:B3", true);

            // Veri tablosunu görüntüleme
            chart.ShowDataTable = true;

            // Grafik Veri Tablosunu Alma
            ChartDataTable chartTable = chart.ChartDataTable;

            // Grafik Veri Tablosu özelliklerini ayarlama
            chartTable.Font.Color = Color.Red;
            chartTable.AutoScaleFont = true;
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = true;
            chartTable.HasBorderOutline = true;
            chartTable.ShowLegendKey = false;

            // Excel dosyasını kaydetme
            workbook.Save("ChartDataTableExample.xlsx");
            workbook.Save("ChartDataTableExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


