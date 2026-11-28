---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesLayoutProperties özelliği. Tüm ortalama noktaları bağlayan çizginin gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

Tüm ortalama noktalarını birleştiren çizginin gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool ShowMeanLine { get; set; }
```

### Açıklamalar

Yalnızca BoxWhisker grafiğinde çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kutu ve bıyık grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // Bir kutu ve bıyık grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe seri ekle
            chart.NSeries.Add("A1:A7", true);

            // İlk seriyi al
            Series series = chart.NSeries[0];

            // Düzen özelliklerine eriş
            SeriesLayoutProperties layout = series.LayoutProperties;

            // ShowMeanLine özelliğini göster
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // ShowMeanLine'ı true olarak ayarla
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // Çalışma kitabını kaydedin
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


