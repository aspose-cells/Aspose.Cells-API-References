---
title: "Series.SecondPlotSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Seri özelliği. Bir pasta grafiğinin ikincil bölümü ya da pasta grafiğinin çubuğu boyutunu, birincil pastanın boyutunun yüzdesi olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir"
type: docs
url: /tr/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

İkincil dilimin (pie of pie grafiği veya bar of pie grafiği) boyutunu, birincil dilimin boyutunun yüzdesi olarak döndürür veya ayarlar. 5 ile 200 arasında bir değer olabilir.

```csharp
public short SecondPlotSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pasta grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi al
            Series series = chart.NSeries[0];

            // SecondPlotSize özelliğini ayarlayın (ikinci grafikte gösterilecek pastanın yüzdesi)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


